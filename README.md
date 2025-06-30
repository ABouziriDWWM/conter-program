# 🔢 Compteur en JavaScript

Une petite application web qui permet d'incrémenter, décrémenter et réinitialiser un compteur via des boutons. Le projet est réalisé avec **JavaScript pur**, sans bibliothèque externe.

## 🚀 Fonctionnalités

- ✅ Incrémenter le compteur
- ✅ Décrémenter le compteur
- ✅ Réinitialiser le compteur à zéro
- ✅ Mise à jour en temps réel de l'affichage

## 📄 Exemple de structure HTML

```html
<button id="decreaseBtn">-</button>
<button id="resetBtn">Reset</button>
<button id="increaseBtn">+</button>
<p id="countLabel">0</p>
💻 Code JavaScript
javascript
Copier
Modifier
const decreaseBtn = document.getElementById("decreaseBtn");
const resetBtn = document.getElementById("resetBtn");
const increaseBtn = document.getElementById("increaseBtn");
const countLabel = document.getElementById("countLabel");

let count = 0;

increaseBtn.onclick = function () {
  count++;
  countLabel.textContent = count;
};

decreaseBtn.onclick = function () {
  count--;
  countLabel.textContent = count;
};

resetBtn.onclick = function () {
  count = 0;
  countLabel.textContent = count;
};
⚙️ Instructions
1️⃣ Ajoute le code HTML dans ton fichier .html
2️⃣ Ajoute le JavaScript dans un fichier .js et relie-le dans ton HTML :

html
Copier
Modifier
<script src="script.js"></script>
3️⃣ Ouvre le fichier dans ton navigateur
4️⃣ Clique sur les boutons pour manipuler le compteur

💡 Améliorations possibles
Ajouter un style CSS pour un meilleur design

Désactiver le bouton "-" lorsque le compteur est à zéro (pour éviter les nombres négatifs, si souhaité)

Afficher un message ou changer de couleur selon la valeur
