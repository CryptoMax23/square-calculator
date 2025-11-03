square-calculator/
├── main.py
├── README.md
└── requirements.txt
def square_area(side: float) -> float:
    return side * side

def square_perimeter(side: float) -> float:
    return 4 * side

if __name__ == "__main__":
    side = float(input("Longueur du côté du carré : "))
    print(f"Aire : {square_area(side)}")
    print(f"Périmètre : {square_perimeter(side)}")
# 🟩 Square Calculator
Un petit programme Python pour calculer l'aire et le périmètre d’un carré.

## Utilisation
```bash
python main.py

---

### 🖥️ **Projet 2 : "square-web"**
Un mini site web affichant un carré coloré dont la taille est réglable.  
**Langage :** HTML + CSS + JS  

```bash
square-web/
├── index.html
├── style.css
└── script.js
<!DOCTYPE html>
<html>
<head>
  <title>Square Web</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>🟩 Carré interactif</h1>
  <input type="range" id="size" min="50" max="300" value="150">
  <div id="square"></div>
  <script src="script.js"></script>
</body>
</html>
body {
  font-family: sans-serif;
  text-align: center;
  margin-top: 50px;
}
#square {
  margin: 30px auto;
  background-color: limegreen;
  width: 150px;
  height: 150px;
}
const square = document.getElementById("square");
document.getElementById("size").addEventListener("input", (e) => {
  const size = e.target.value;
  square.style.width = `${size}px`;
  square.style.height = `${size}px`;
});
