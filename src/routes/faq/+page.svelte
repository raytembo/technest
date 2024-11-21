<script>
    // Data for FAQs
    const faqs = [
      {
        question: "What is TechNest?",
        answer:
          "TechNest is your one-stop shop for the latest tech gadgets, accessories, and smart solutions.",
      },
      {
        question: "What products do you offer?",
        answer:
          "We offer a wide range of products including smartphones, laptops, accessories, and smart home devices.",
      },
      {
        question: "How do I place an order?",
        answer:
          "Simply browse our product catalog, add items to your cart, and proceed to checkout for a seamless shopping experience.",
      },
      {
        question: "What is your return policy?",
        answer:
          "You can return most items within 30 days of purchase for a full refund or exchange. Please check our return policy page for more details.",
      },
      {
        question: "How can I contact customer support?",
        answer:
          "You can reach us via email at support@technest.com or call us at 1-800-TECH-NEST.",
      },
    ];
  
    // Track which FAQ is expanded
    let expandedIndex = null;
  
    // Toggle FAQ visibility
    const toggleFAQ = (index) => {
      expandedIndex = expandedIndex === index ? null : index;
    };
  </script>
  
  <main>
    <h1>Frequently Asked Questions</h1>
    <p>Have questions about TechNest? Find answers below!</p>
  
    <div class="faq-container">
      {#each faqs as faq, index}
        <div class="faq-item">
          <h2 on:click={() => toggleFAQ(index)} class="faq-question">
            {faq.question}
            <span class="arrow">{expandedIndex === index ? "▲" : "▼"}</span>
          </h2>
          {#if expandedIndex === index}
            <p class="faq-answer">{faq.answer}</p>
          {/if}
        </div>
      {/each}
    </div>
  </main>
  
  <style>
    main {
      font-family: Arial, sans-serif;
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
      text-align: center;
    }
  
    h1 {
      font-size: 2.5rem;
      color: #333;
    }
  
    p {
      color: #666;
      margin-bottom: 20px;
    }
  
    .faq-container {
      margin-top: 20px;
      text-align: left;
    }
  
    .faq-item {
      margin-bottom: 15px;
      border: 1px solid #ddd;
      border-radius: 5px;
      overflow: hidden;
      background: #f9f9f9;
    }
  
    .faq-question {
      margin: 0;
      padding: 15px;
      background-color: #007bff;
      color: white;
      cursor: pointer;
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 1.1rem;
    }
  
    .faq-answer {
      margin: 0;
      padding: 15px;
      color: #333;
      background: white;
    }
  
    .arrow {
      font-size: 0.9rem;
    }
  
    .faq-question:hover {
      background-color: #0056b3;
    }
  </style>
  