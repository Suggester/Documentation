<style>
  .cover-main {
    width: 80%; /* Base width */
    max-width: 1200px; /* Max width on larger screens to avoid too wide content */
    padding: 20px;
    text-align: left;
    margin: 0 auto; /* Centers the content */
  }

  .cover-main h1 {
    font-size: 3em; /* Larger font size for headings */
    margin-bottom: 0.3em;
  }

  .cover-main h1 .brand,
  .cover-main h1 .doc {
    color: #2ecc71; /* Green color for brand */
    font-weight: bold;
  }

  .cover-main p {
    font-size: 1.3em;
    width: 100%; /* Full width */
    margin-bottom: 2em;
  }

  .cover-main a.button {
    display: inline-block;
    margin-right: 16px;
    padding: 12px 24px;
    border-radius: 0px;
    text-decoration: none;
    font-weight: bold;
    color: white;
    background-color: #5865F2; /* Customize background color for the button */
  }

  /* Mobile responsiveness */
  @media (max-width: 768px) {
    .cover-main {
      width: 90%; /* 90% width for mobile */
      padding: 20px;
    }

    .cover-main h1 {
      font-size: 2.5em;
    }

    .cover-main p {
      font-size: 1.1em;
    }

    .cover-main a.button {
      padding: 10px 20px;
      font-size: 1em;
    }
  }

  /* Extra small mobile (portrait phones) */
  @media (max-width: 480px) {
    .cover-main {
      width: 95%; /* 95% width on very small screens */
      padding: 10px;
    }

    .cover-main h1 {
      font-size: 2em;
    }

    .cover-main p {
      font-size: 1em;
    }

    .cover-main a.button {
      padding: 8px 18px;
      font-size: 0.9em;
    }
  }
</style>

<div class="cover-main">
  <h1>
    <span class="brand">Suggester</span><br>
    <span class="doc">Documentation</span>
  </h1>
  <p>Suggester is a Discord application helping communities manage feedback from their members, with the usage of a modern suggestion system and its granular configuration elements.</p>

  <a class="get-started-button" href="/#/README">
    Get Started
  </a>
</div>
