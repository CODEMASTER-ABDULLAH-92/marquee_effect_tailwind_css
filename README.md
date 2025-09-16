# 🎞️ Marquee Animation using CSS & Tailwind

This project demonstrates a simple **marquee animation** (text scrolling effect) using **CSS keyframes** and **Tailwind CSS**.

---

## 📂 Project Structure

```plaintext
project/
├── index.html      # Main HTML file
├── style.css       # Custom CSS for animations
└── README.md       # Documentation
```
## 📂 HTML CODE

```plaintext
    <div class="flex gap-5">
      <div class="animate-marquee py-12 whitespace-nowrap">
        <span class="mx-4 text-4xl">Marquee Item 1</span>
        <span class="mx-4 text-4xl">Marquee Item 2</span>
        <span class="mx-4 text-4xl">Marquee Item 3</span>
        <span class="mx-4 text-4xl">Marquee Item 4</span>
        <span class="mx-4 text-4xl">Marquee Item 5</span>
      </div>

      <div class="absolute animate-marquee2 py-12 whitespace-nowrap">
        <span class="mx-4 text-4xl">Marquee Item 1</span>
        <span class="mx-4 text-4xl">Marquee Item 2</span>
        <span class="mx-4 text-4xl">Marquee Item 3</span>
        <span class="mx-4 text-4xl">Marquee Item 4</span>
        <span class="mx-4 text-4xl">Marquee Item 5</span>
      </div>
    </div>
```
## 📂 CSS CODE
```plaintext
.animate-marquee {
  animation-name: marquee;
  animation-duration: 4s;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}

.animate-marquee2 {
  animation-name: marquee2; /* ✅ FIXED */
  animation-duration: 4s;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}

@keyframes marquee {
  0% {
    transform: translateX(0%);
  }
  100% {
    transform: translateX(-100%);
  }
}

@keyframes marquee2 {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(0%);
  }
}
```
