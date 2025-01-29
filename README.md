# GestureFlow PDF Viewer  

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.7%2B-orange)](https://opencv.org)

**Une visionneuse PDF innovante avec contrôle gestuel et interface moderne**  

<div align="center">
  <img src="screenshot.png" alt="Interface" width="600">
</div>

## ✨ Fonctionnalités

- **📁 Chargement PDF**  
  Ouvrez des fichiers PDF depuis l'interface ou par glisser-déposer.

- **👆 Contrôle gestuel intuitif**  
  Naviguez, zoomez et contrôlez le curseur avec des gestes de la main :
  - Pincement pour zoomer
  - Poing fermé → Page suivante
  - Main ouverte → Page précédente

- **🎮 Interface optimisée**  
  - Zoom tactile (molette souris)  
  - Navigation rapide entre pages  
  - Affichage responsive HD  

- **⚙️ Multi-OS**  
  Supporte Windows, Linux et macOS.

- **🎨 UI personnalisable**  
  Thèmes sombre/clair et styles CSS modifiables.

## 🚀 Installation

### Prérequis
- Python 3.9+
- Webcam
- Poppler-utils (pour la conversion PDF)

### Étapes
1. Installer les dépendances système :
   ```bash
   # Ubuntu/Debian
   sudo apt install poppler-utils

   # Windows : Télécharger Poppler et ajouter au PATH
   ```

2. Cloner le dépôt :
   ```bash
   git clone https://github.com/TitanSage02/gestureflow-pdf-viewer.git
   cd gestureflow-pdf-viewer
   ```

3. Installer les dépendances Python :
   ```bash
   pip install -r requirements.txt
   ```

## 🖥️ Utilisation

1. Lancer l'application :
   ```bash
   python main.py
   ```

2. Charger un PDF :
   - Cliquer sur "📂 Ouvrir PDF"
   - Sélectionner un fichier

3. Commandes gestuelles :
   | Geste                  | Action                |
   |------------------------|-----------------------|
   | 🤏 Pincement (serré)   | Zoom -                |
   | 🤏 Pincement (large)   | Zoom +                |
   | ✊ Poing fermé          | Page suivante         |
   | 🖐 Main ouverte         | Page précédente       |
   | 👆 Index levé          | Contrôle du curseur   |

## 📦 Dépendances

| Package       | Version | Usage                     |
|---------------|---------|---------------------------|
| PySide6       | 6.4+    | Interface graphique       |
| pdf2image     | 1.16+   | Conversion PDF vers image |
| opencv-python | 4.7+    | Traitement vidéo          |
| cvzone        | 1.5+    | Détection de gestes       |
| pyautogui     | 0.9+    | Contrôle du curseur       |

## 🧩 Structure du Projet

```
gestureflow-pdf-viewer/
├── main.py            # Point d'entrée principal
├── requirements.txt   # Dépendances Python
├── ui/                | Fichiers d'interface
   └── icons/         | Icônes et images
└── docs/              # Documentation technique
```

## 🤝 Contribution

1. Forker le projet
2. Créer une branche :
   ```bash
   git checkout -b feature/nouvelle-fonctionnalite
   ```
3. Commiter les changements
4. Ouvrir une Pull Request

## 📄 License

Distribué sous licence MIT. Voir `LICENSE` pour plus de détails.

## 🙏 Remerciements

- Bibliothèque [CVZone](https://github.com/cvzone/cvzone) pour la détection de mains
- [PySide6](https://www.qt.io/qt-for-python) pour l'interface Qt moderne
- Communauté Open Source pour les outils de conversion PDF