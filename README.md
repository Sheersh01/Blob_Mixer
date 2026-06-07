# Blobmixer 🎨✨

An interactive, 3D web experience showcasing dynamic, beautifully shaded blobs. Built with **Three.js**, **GSAP**, and custom shaders, this project allows users to scroll through a collection of unique, animated 3D blobs ("Color Fusion", "Purple Mirror", and "Alien Goo"), each featuring distinct textures, materials, and environment maps.

## ✨ Features

- **Interactive 3D Blobs:** A customizable 3D sphere that morphs its shape using vertex shaders.
- **Custom Shader Materials:** Utilizes `three-custom-shader-material` to blend standard Three.js physically based rendering (PBR) with custom vertex displacement.
- **Smooth Animations:** Powered by **GSAP**, transitioning between different blob states (color, shape frequency, camera rotation, and background) is buttery smooth.
- **Dynamic 3D Text:** Implements `troika-three-text` for sharp, performant 3D typography that animates alongside the blobs.
- **HDRI Lighting:** Uses HDR environment maps via `RGBELoader` for realistic reflections and lighting.

## 🛠️ Technologies Used

- **[Three.js](https://threejs.org/)** - Core 3D rendering engine
- **[GSAP](https://gsap.com/)** - Advanced animation library for smooth transitions
- **[Vite](https://vitejs.dev/)** - Next-generation frontend tooling and bundler
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework for UI overlay
- **three-custom-shader-material** - For extending Three.js materials with custom GLSL
- **troika-three-text** - High-quality text rendering in 3D space
- **GLSL** - Custom vertex shaders for the blob displacement

## 🚀 Getting Started

Follow these steps to run the project locally.

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Sheersh01/Blob_Mixer.git
   cd blob-mixer
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. Open your browser and visit the URL provided by Vite (usually `http://localhost:5173/`).

## 🎮 How to Use

- **Scroll:** Use your mouse wheel or trackpad to scroll up and down. This will trigger the animation, morphing the blob into its next state, changing the background, and updating the 3D text.

## 📁 Project Structure

- `index.html`: Main HTML entry point with UI overlay.
- `main.js`: Core Three.js logic, scene setup, and GSAP animations.
- `shaders/`: Contains custom GLSL shaders (`vertex.glsl`, `textVertex.glsl`).
- `public/`: Static assets like textures, gradients, and fonts.
- `style.css`: Custom CSS for UI elements.
