<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>CABI Profile - Matte Black with Silver</title>

  <!-- Google Fonts Montserrat -->
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet" />

  <style>
    /* Smooth scroll */
    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Montserrat', sans-serif;
      margin: 40px;
      background-color: #121212; /* Matte black background */
      color: #c0c0c0; /* Silver text */
      display: flex;
      justify-content: center;
      min-height: 100vh;
    }

    .container {
      max-width: 900px;
      display: flex;
      gap: 50px;
      align-items: flex-start;
      background-color: #1c1c1c; /* Dark charcoal container */
      box-shadow: 0 12px 30px rgba(192, 192, 192, 0.15); /* subtle silver shadow */
      border-radius: 20px;
      padding: 40px 50px;
      animation: fadeIn 1s ease forwards;
    }

    /* Fade-in animation */
    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .left {
      max-width: 320px;
      text-align: center;
      background-color: #242424;
      border-radius: 20px;
      padding: 20px;
      box-shadow: 0 0 15px #c0c0c088; /* faint silver glow */
    }

    h2.logo {
      color: #c0c0c0; /* silver */
      font-weight: 900;
      font-size: 2rem;
      margin-bottom: 30px;
      letter-spacing: 4px;
      text-transform: uppercase;
    }

    .photo {
      width: 100%;
      max-width: 320px;
      border-radius: 50%;
      border: 4px solid #c0c0c0cc; /* solid silver border with transparency */
      box-shadow: 0 0 10px #c0c0c0bb;
      object-fit: cover;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .photo:hover {
      transform: scale(1.05);
      box-shadow: 0 0 20px #c0c0c0dd;
    }

    .github-button {
      display: inline-block;
      margin-top: 25px;
      padding: 12px 30px;
      font-size: 16px;
      font-weight: 700;
      color: #121212; /* matte black text */
      background: linear-gradient(135deg, #d9d9d9, #bfbfbf);
      border-radius: 30px;
      text-decoration: none;
      box-shadow: 0 6px 15px #c0c0c090;
      transition: background 0.3s ease, box-shadow 0.3s ease, color 0.3s ease;
      font-family: 'Montserrat', sans-serif;
    }

    .github-button:hover {
      background: linear-gradient(135deg, #bfbfbf, #d9d9d9);
      box-shadow: 0 10px 25px #c0c0c0cc;
      color: #121212;
    }

    /* Scroll reveal hidden states */
    .left.hidden {
      opacity: 0;
      transform: translateX(-50px);
      transition: opacity 0.7s ease, transform 0.7s ease;
    }
    .right.hidden {
      opacity: 0;
      transform: translateX(50px);
      transition: opacity 0.7s ease, transform 0.7s ease;
    }

    /* Scroll reveal visible states */
    .left.visible,
    .right.visible {
      opacity: 1;
      transform: translateX(0);
    }

    .right {
      max-width: 560px;
    }

    .right h1 {
      font-weight: 900;
      margin-bottom: 12px;
      font-size: 2.7rem;
      color: #c0c0c0; /* silver heading */
    }

    .right h3 {
      font-weight: 700;
      margin-top: 25px;
      margin-bottom: 15px;
      font-size: 1.3rem;
      color: #d8d8d8; /* lighter silver */
      border-left: 6px solid #c0c0c0;
      padding-left: 16px;
    }

    .right p {
      line-height: 1.8;
      margin-bottom: 22px;
      color: #b0b0b0; /* medium silver gray */
      font-size: 1.05rem;
    }

    /* Responsive design */
    @media (max-width: 768px) {
      body {
        margin: 20px;
      }
      .container {
        flex-direction: column;
        padding: 30px 20px;
      }
      .left,
      .right {
        max-width: 100%;
      }
      .left {
        margin-bottom: 35px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="left">
      <h2 class="logo">CABI</h2>
      <img
        src="https://i.ibb.co/2F8jFHf/photo-profile.jpg"
        alt="Profile Photo"
        class="photo"
      />
      <a
        href="https://github.com/cabl0-o"
        target="_blank"
        rel="noopener noreferrer"
        class="github-button"
        >View My GitHub Profile</a
      >
    </div>
    <div class="right">
      <h1>Hi, I'm Karylle!</h1>
      <h3>Bachelor of Science in Information Technology</h3>
      <h3>Contact</h3>
      <p>Email: cabridokarylle@gmail.com</p>
      <p>Phone: 0995-145-4499</p>
      <p>Location: Brgy. San Agustin, Alaminos, Laguna.</p>
      <h3>Lorem Ipsum</h3>
      <p>
        Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus ex sapien vitae pellentesque sem placerat. In id cursus mi pretium tellus duis convallis. Tempus leo eu aenean sed diam urna tempor. Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra inceptos himenaeos.
      </p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus ex sapien vitae pellentesque sem placerat. In id cursus mi pretium tellus duis convallis. Tempus leo eu aenean sed diam urna tempor. Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra inceptos himenaeos.
      </p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus ex sapien vitae pellentesque sem placerat. In id cursus mi pretium tellus duis convallis. Tempus leo eu aenean sed diam urna tempor. Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra inceptos himenaeos.
      </p>
    </div>
  </div>

  <!-- Scroll reveal script -->
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const observerOptions = {
        root: null,
        rootMargin: '0px',
        threshold: 0.1
      };

      const observerCallback = (entries, observer) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.classList.add('visible');
            observer.unobserve(entry.target);
          }
        });
      };

      const observer = new IntersectionObserver(
        observerCallback,
        observerOptions
      );

      document.querySelectorAll('.left, .right').forEach(elem => {
        elem.classList.add('hidden'); // Start hidden
        observer.observe(elem);
      });
    });
  </script>
</body>
</html>

