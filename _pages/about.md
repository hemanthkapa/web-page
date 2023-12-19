---
layout: page
title: About
favicon: 🎨
---

> 💡 Crafting an ornament named **Life** by beautifully arranging beads called **Memories**.


<div class="about-content" style="display: flex; align-items: flex-start; gap: 30px; margin-top: 20px;">
    <div style="flex: 1;">
        <img src="assets/images/IMG_7489.jpeg" alt="Image" style="width: 100%; height: auto; border-radius: 10px;">
    </div>
    <div style="flex: 2; padding: 10px; background-color: rgba(156, 213, 56, .08); border-radius: 10px;">
        <p>I'm a 19-year-old from India, currently delving into the realms of Computer Science and Neuroscience at Dickinson College 🎓. Fascinated by the uncharted territories of life, I'm passionately exploring the intricate world of aging, AI 🧠, and medical technology 🔬. My mission is simple yet profound: solve hard and non-obvious problems that uplift and transform human lives.</p>

        <p>Somethings I'm proud of:</p>
        <ul>
            <li>🏅 Emergent Ventures Grantee</li>
            <li>📚 Next Genius Scholar 2023</li>
            <li>🤺 State-level Fencer</li>
        </ul>     
    </div>

    <div style="margin-top: 20px;">
        <p>Connect with me on social media:</p>
        <a href="https://www.instagram.com/hemanth.kapa/" target="_blank" style="margin-right: 10px;">Instagram</a>
        <a href="https://www.linkedin.com/in/hemanth-kapa/" target="_blank" style="margin-right: 10px;">LinkedIn</a>
        <a href="https://twitter.com/kapahemanth" target="_blank">Twitter</a>
    </div>
</div>


<style>

    .about-content {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
}

.about-content > div {
  flex: 1 1 100%; /* Make each child take full width on smaller screens */
}

@media (min-width: 768px) { /* Adjust this breakpoint as needed */
  .about-content {
    align-items: flex-start;
  }
  
  .about-content > div:first-child {
    flex: 1;
  }

  .about-content > div:not(:first-child) {
    flex: 2;
  }
}

.about-content img {
        width: 100%; /* Full width of its parent container */
        height: auto; /* Maintain aspect ratio */
        border-radius: 10px;
        max-width: 300px; /* Default max width for mobile */
    }

    @media (min-width: 768px) { /* Desktop and larger screens */
        .about-content img {
            max-width: 600px; /* Larger max width for desktop */
        }

        .about-content {
            align-items: flex-start;
        }

        .about-content > div:first-child {
            flex: 1;
        }

        .about-content > div:not(:first-child) {
            flex: 2;
        }
    }

    .about-content p, .about-content ul {
        font-size: 1em; 
        line-height: 1.6;
    }

    @media (max-width: 768px) {
        .about-content p, .about-content ul {
            font-size: 0.9em; /* Smaller font size for mobile */
        }
    }

    .social-media-links a {
        color: #000000;
        text-decoration: none;
        padding: 5px; /* Easier to tap on mobile */
    }

    .social-media-links a:hover, .social-media-links a:focus {
        text-decoration: underline;
    }
</style>

</style>
