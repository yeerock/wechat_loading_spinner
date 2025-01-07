# WeChat-Inspired Loader Spinner Animation

This project replicates the minimalist and elegant loading spinner animation inspired by the WeChat app. It features a smooth, continuously rotating circular loader paired with a "Loading..." text, both enclosed in a compact, semi-transparent dark box for a clean and modern appearance. Designed with HTML and CSS, this lightweight solution is perfect for applications or websites that aim to enhance their user experience with a polished, professional touch. The animation is fully responsive and easy to integrate, making it an excellent choice for preloading screens or data fetching indicators.

## Features
- Smooth infinite rotation animation for the spinner.
- Minimalistic design styled after the WeChat aesthetic.
- Responsive and lightweight implementation using pure HTML and CSS.
- Easy to customize and integrate into any web project.

## Preview
To see the animation in action, add the following code to your project and open it in a browser:

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      background: #f5f5f5;
    }

    .loader-box {
      width: 120px;
      height: 120px;
      background: rgba(0, 0, 0, 0.7);
      border-radius: 10px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 12px;
    }

    .spinner {
      width: 36px;
      height: 36px;
      border: 3px solid rgba(255, 255, 255, 0.3);
      border-top: 3px solid white;
      border-radius: 50%;
      animation: spin 1s linear infinite;
    }

    .loader-text {
      color: white;
      font-family: system-ui, -apple-system, sans-serif;
      font-size: 14px;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
  </style>
</head>
<body>
  <div class="loader-box">
    <div class="spinner"></div>
    <div class="loader-text">Loading...</div>
  </div>
</body>
</html>
