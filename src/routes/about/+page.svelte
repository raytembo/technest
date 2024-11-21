<script>
    const teamMembers = [
      { name: 'Ray Johnson', position: 'Founder & CEO', image: 'https://via.placeholder.com/150' },
      { name: 'Alice Brown', position: 'CTO', image: 'https://via.placeholder.com/150' },
      { name: 'John Smith', position: 'Lead Developer', image: 'https://via.placeholder.com/150' },
    ];
  </script>
  
  <main>
    <!-- Hero Section -->
    <section class="hero">
      <h1>About TechNest</h1>
      <p>Innovation at the heart of every solution. Explore our story and mission to empower the tech community.</p>
    </section>
  
    <!-- Company Overview Section -->
    <section class="overview">
      <h2>Company Overview</h2>
      <p>
        At TechNest, we believe in transforming the way people interact with technology. Founded in 2022, our company has been at the forefront of providing cutting-edge tech solutions, offering everything from innovative gadgets to smart home products. 
      </p>
      <p>
        Our goal is to bring technology closer to you, making it simpler, smarter, and more accessible for everyone.
      </p>
    </section>
  
    <!-- Mission Section -->
    <section class="mission">
      <h2>Our Mission</h2>
      <p>
        To empower individuals and businesses with the latest technology solutions that enhance productivity, creativity, and connectivity. 
        We are committed to delivering value, fostering innovation, and building a sustainable tech-driven future.
      </p>
    </section>
  
    <!-- Team Section -->
    <section class="team">
      <h2>Meet Our Team</h2>
      <div class="team-grid">
        {#each teamMembers as member}
          <div class="team-card">
            <img src={member.image} alt={member.name} />
            <h3>{member.name}</h3>
            <p>{member.position}</p>
          </div>
        {/each}
      </div>
    </section>
  
    <!-- Contact Us Section -->
    <section class="contact">
      <h2>Contact Us</h2>
      <p>We'd love to hear from you! Whether you have questions, feedback, or collaboration ideas, feel free to reach out.</p>
      <form>
        <label for="name">Name</label>
        <input type="text" id="name" placeholder="Your Name" />
  
        <label for="email">Email</label>
        <input type="email" id="email" placeholder="Your Email" />
  
        <label for="message">Message</label>
        <textarea id="message" placeholder="Your Message"></textarea>
  
        <button type="submit">Send Message</button>
      </form>
    </section>
  </main>
  
  <style>
    /* General Styles */
    main {
      font-family: Arial, sans-serif;
      margin: 0 auto;
      padding: 20px;
      max-width: 800px;
      line-height: 1.6;
    }
  
    section {
      margin-bottom: 40px;
    }
  
    h1, h2 {
      text-align: center;
      color: #333;
    }
  
    p {
      color: #555;
      text-align: justify;
    }
  
    /* Hero Section */
    .hero {
      text-align: center;
      padding: 30px 20px;
      background: #f0f4f8;
      border-radius: 8px;
    }
  
    .hero h1 {
      margin-bottom: 10px;
      font-size: 2.5em;
      color: #007BFF;
    }
  
    .hero p {
      font-size: 1.2em;
    }
  
    /* Team Section */
    .team-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
    }
  
    .team-card {
      text-align: center;
      padding: 15px;
      border: 1px solid #ddd;
      border-radius: 8px;
      background-color: #f9f9f9;
    }
  
    .team-card img {
      border-radius: 50%;
      width: 100px;
      height: 100px;
      margin-bottom: 10px;
    }
  
    .team-card h3 {
      margin: 10px 0 5px;
      font-size: 1.2em;
      color: #007BFF;
    }
  
    .team-card p {
      color: #555;
    }
  
    /* Contact Form */
    .contact form {
      display: flex;
      flex-direction: column;
    }
  
    .contact label {
      margin-top: 10px;
      font-weight: bold;
    }
  
    .contact input,
    .contact textarea {
      margin-top: 5px;
      padding: 10px;
      border: 1px solid #ddd;
      border-radius: 5px;
      font-size: 1em;
    }
  
    .contact textarea {
      resize: vertical;
    }
  
    .contact button {
      margin-top: 15px;
      padding: 10px 15px;
      border: none;
      border-radius: 5px;
      background-color: #007BFF;
      color: white;
      font-size: 1em;
      cursor: pointer;
    }
  
    .contact button:hover {
      background-color: #0056b3;
    }
  </style>
  