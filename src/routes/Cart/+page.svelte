<script>
    
    let cart = [];
  
    const addToCart = (product) => {
      cart = [...cart, product];
    };
  </script>
  
  <main>
    <h1>Tech Nest</h1>
    <p>Explore our latest tech gadgets across categories!</p>
    
    
    <aside>
      <h2>Shopping Cart</h2>
      {#if cart.length > 0}
        <ul>
          {#each cart as item}
            <li>{item.name} - ${item.price}</li>
          {/each}
        </ul>
      {:else}
        <p>Your cart is empty!</p>
      {/if}
    </aside>
  </main>
  
  <style>
    main {
      display: flex;
      flex-direction: column;
      align-items: center;
      font-family: Arial, sans-serif;
    }
    aside {
      margin-top: 20px;
      border-top: 1px solid #ccc;
      padding-top: 10px;
      width: 50%;
      text-align: left;
    }
  </style>
  