# Peer-graded Assignment — Option 1: Demo portfolio (coded from scratch)

## Live site
https://21011612.github.io/Advanced-Styling-with-Responsive-Design-Peer-graded-Assignment-Final-Project-Photo-Gallery/

## Overview
Mobile-first gallery, 3 breakpoints (mobile / ≥772px / ≥992px), tôn trọng user preferences (`prefers-reduced-motion`, `prefers-color-scheme: dark`).

- **Mobile:** grid 1 cột, `gap: 10px`.
- **Tablet (≥772px):** grid 2 cột; `figure:last-of-type { grid-column: 1 / -1 }`; bo tròn (circle).
- **Large (≥992px):** `figure:nth-child(3n) { grid-column: 1 / -1 }`; bỏ bo tròn.
- Không dùng `max-width` cho breakpoint.

## Evidence (theo yêu cầu)
- **W3C HTML Validator:** xem file `w3c-validation.txt` (kéo từ W3C) hoặc chạy lại trực tiếp với URL.
- **Responsive:** 3 ảnh chụp (mobile / 772px / 992+px) hoặc 1 video ngắn (thêm vào phần nộp Coursera).
- **Well-styled:** CSS có variables, media queries, grid span theo vị trí.

## Four “extras” (và code)
1) **Dark mode** — `prefers-color-scheme: dark`  
   Figures chuyển **nền tối**, **chữ sáng (vàng nhạt)**, **viền đen**.
2) **Reduced motion** — `prefers-reduced-motion: reduce`  
   Tắt `scroll-behavior: smooth`; disable animation/transition.
3) **Skip link + focus visible**  
   `<a class="skip" href="#main">Skip to content</a>`; đảm bảo outline focus rõ.
4) **Grid nâng cao**  
   Tablet: `last-of-type` span 2 cột; Large: `nth-child(3n)` span 2 cột.

## How to validate (tóm tắt)
- HTML: https://validator.w3.org/  → nhập URL site.  
- A11y/contrast: https://wave.webaim.org/  → nhập URL site (hoặc dùng extension).  
- Test reduced-motion/dark mode: đổi setting OS, hoặc DevTools emulation.

