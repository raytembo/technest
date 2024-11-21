<script>
    // Mock blog data
    let posts = [
      {
        id: 1,
        title: "Top 10 Tech Gadgets of 2024",
        date: "November 20, 2024",
        summary: "Discover the hottest gadgets that will redefine the tech industry this year.",
        content: "In this article, we explore the most innovative tech gadgets of 2024, including smart devices, AI-powered tools, and futuristic accessories.",
      },
      {
        id: 2,
        title: "Why Smart Homes Are the Future",
        date: "November 18, 2024",
        summary: "Explore how smart home technology is making our lives easier and more connected.",
        content: "Smart homes are becoming a staple in modern living. From voice-activated controls to energy-efficient solutions, find out how they’re shaping the future.",
      },
      {
        id: 3,
        title: "AI and the Evolution of Tech",
        date: "November 15, 2024",
        summary: "An in-depth look at how AI is transforming industries across the globe.",
        content: "Artificial Intelligence is no longer a buzzword—it’s a reality. This article dives deep into the latest AI advancements and their impact on the tech ecosystem.",
      },
    ];
  
    let selectedPost = null;
  
    // Functions to handle post selection and back navigation
    const selectPost = (post) => {
      selectedPost = post;
    };
  
    const goBack = () => {
      selectedPost = null;
    };
  </script>
  
  <main>
    <!-- Hero Section -->
    <section class="hero">
      <h1>Welcome to the Tech Nest Blog</h1>
      <p>Your source for the latest tech trends, insights, and innovations.</p>
    </section>
  
    <!-- Blog Section -->
    {#if selectedPost}
      <!-- Single Post View -->
      <section class="single-post">
        <button on:click={goBack}>&larr; Back to All Posts</button>
        <h2>{selectedPost.title}</h2>
        <p class="date">{selectedPost.date}</p>
        <p>{selectedPost.content}</p>
      </section>
    {:else}
      <!-- Blog List View -->
      <section class="blog-list">
        <h2>Latest Posts</h2>
        <ul>
          {#each posts as post}
            <!-- svelte-ignore a11y_no_noninteractive_element_interactions -->
            <!-- svelte-ignore a11y_click_events_have_key_events -->
            <li class="blog-card" on:click={() => selectPost(post)}>
              <h3>{post.title}</h3>
              <p class="date">{post.date}</p>
              <p>{post.summary}</p>
              <button>Read More</button>
            </li>
          {/each}
        </ul>
      </section>
    {/if}
  </main>
  
  <style>
    /* Global Styles */
    main {
      font-family: Arial, sans-serif;
      padding: 20px;
      max-width: 800px;
      margin: auto;
    }
  
    h1, h2, h3 {
      color: #333;
    }
  
    p {
      color: #555;
    }
  
    button {
      background-color: #007BFF;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 14px;
    }
  
    button:hover {
      background-color: #0056b3;
    }
  
    /* Hero Section */
    .hero {
      text-align: center;
      padding: 40px 20px;
      background-color: #f9f9f9;
      border-radius: 8px;
      margin-bottom: 20px;
    }
  
    /* Blog List Section */
    .blog-list ul {
      list-style: none;
      padding: 0;
    }
  
    .blog-card {
      border: 1px solid #ddd;
      border-radius: 8px;
      padding: 20px;
      margin-bottom: 20px;
      background-color: #fff;
      transition: box-shadow 0.3s;
      cursor: pointer;
    }
  
    .blog-card:hover {
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
  
    .blog-card h3 {
      margin-bottom: 10px;
    }
  
    .blog-card .date {
      color: #888;
      font-size: 12px;
      margin-bottom: 15px;
    }
  
    .blog-card button {
      margin-top: 10px;
    }
  
    /* Single Post Section */
    .single-post {
      padding: 20px;
      border: 1px solid #ddd;
      border-radius: 8px;
      background-color: #fff;
    }
  
    .single-post .date {
      color: #888;
      font-size: 12px;
      margin-bottom: 20px;
    }
  </style>
  