<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Grind Lead Motivate | Official Store</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Barlow:wght@300;400;500;600&family=Barlow+Condensed:wght@700;900&display=swap" rel="stylesheet">
<style>
:root{--black:#080808;--dark:#111;--card:#161616;--border:#222;--red:#cc1f1f;--accent:#e8ff00;--white:#f0f0f0;--muted:#666;--success:#00e676;}
*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{background:var(--black);color:var(--white);font-family:"Barlow",sans-serif;overflow-x:hidden;}

nav{position:fixed;top:0;left:0;right:0;z-index:999;display:flex;align-items:center;justify-content:space-between;padding:16px 36px;background:rgba(8,8,8,0.95);backdrop-filter:blur(12px);border-bottom:1px solid var(–border);}
.nav-logo{display:flex;align-items:center;gap:10px;text-decoration:none;}
.nav-logo img{height:36px;object-fit:contain;}
.nav-logo span{font-family:“Bebas Neue”,cursive;font-size:1.3rem;letter-spacing:3px;color:var(–white);}
.nav-links{display:flex;gap:28px;list-style:none;}
.nav-links a{color:var(–muted);text-decoration:none;font-size:0.75rem;letter-spacing:2px;text-transform:uppercase;transition:color 0.2s;}
.nav-links a:hover{color:var(–white);}
.cart-btn{background:var(–red);color:#fff;border:none;padding:10px 22px;font-family:“Barlow Condensed”,sans-serif;font-weight:700;font-size:0.82rem;letter-spacing:2px;text-transform:uppercase;cursor:pointer;transition:all 0.2s;position:relative;}
.cart-btn:hover{background:#e02222;}
.cart-count{position:absolute;top:-6px;right:-6px;background:var(–accent);color:var(–black);border-radius:50%;width:18px;height:18px;font-size:0.65rem;display:none;align-items:center;justify-content:center;font-weight:700;}

.hero{min-height:100vh;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;padding:120px 40px 80px;position:relative;overflow:hidden;}
.hero-bg{position:absolute;inset:0;background-size:cover;background-position:center;filter:brightness(0.25);z-index:0;}
.hero-overlay{position:absolute;inset:0;background:radial-gradient(ellipse 80% 60% at 50% 70%,rgba(204,31,31,0.15) 0%,transparent 70%);z-index:1;}
.hero-content{position:relative;z-index:2;}
.hero-glm-logo{height:80px;margin-bottom:24px;filter:drop-shadow(0 0 20px rgba(204,31,31,0.6));animation:fadeUp 0.8s ease both;}
.hero-title{font-family:“Bebas Neue”,cursive;font-size:clamp(3.5rem,11vw,9rem);line-height:0.88;letter-spacing:4px;color:var(–white);animation:fadeUp 0.8s ease 0.1s both;}
.hero-title .red{color:var(–red);}
.hero-sub{margin-top:20px;font-size:0.95rem;color:#aaa;letter-spacing:1px;max-width:480px;line-height:1.7;animation:fadeUp 0.8s ease 0.2s both;}
.hero-cta{margin-top:40px;display:flex;gap:14px;flex-wrap:wrap;justify-content:center;animation:fadeUp 0.8s ease 0.3s both;}
.btn-red{background:var(–red);color:#fff;border:none;padding:15px 38px;font-family:“Barlow Condensed”,sans-serif;font-weight:900;font-size:0.95rem;letter-spacing:3px;text-transform:uppercase;cursor:pointer;text-decoration:none;display:inline-block;transition:all 0.2s;}
.btn-red:hover{background:#e02222;transform:translateY(-2px);}
.btn-outline{background:transparent;color:var(–white);border:1px solid #444;padding:15px 38px;font-family:“Barlow Condensed”,sans-serif;font-weight:700;font-size:0.95rem;letter-spacing:3px;text-transform:uppercase;cursor:pointer;text-decoration:none;display:inline-block;transition:all 0.2s;}
.btn-outline:hover{border-color:var(–red);color:var(–red);}

.mission-bar{background:#0e0000;border-top:2px solid var(–red);border-bottom:2px solid var(–red);padding:20px 40px;text-align:center;}
.mission-bar p{font-size:0.88rem;color:#ddd;letter-spacing:0.5px;line-height:1.8;max-width:860px;margin:0 auto;}
.mission-bar strong{color:var(–accent);}
.mission-bar .mission-icons{display:flex;justify-content:center;gap:36px;margin-top:14px;flex-wrap:wrap;}
.mission-icon{font-size:0.75rem;color:var(–red);letter-spacing:1px;text-transform:uppercase;font-family:“Barlow Condensed”,sans-serif;font-weight:700;}
.mission-icon::before{display:block;font-size:1.5rem;margin-bottom:4px;text-align:center;}

section{padding:90px 36px;}
.section-label{font-family:“Barlow Condensed”,sans-serif;font-size:0.7rem;letter-spacing:5px;color:var(–red);text-transform:uppercase;margin-bottom:10px;}
.section-title{font-family:“Bebas Neue”,cursive;font-size:clamp(2.2rem,5vw,4rem);letter-spacing:2px;line-height:1;margin-bottom:44px;}

#shop{background:var(–dark);}
.shop-header{text-align:center;margin-bottom:50px;}
.shipping-notice{background:#0a0a00;border:1px solid #2a2800;padding:14px 20px;text-align:center;font-size:0.8rem;color:#b0a030;margin-bottom:36px;max-width:800px;margin-left:auto;margin-right:auto;letter-spacing:0.5px;}
.shipping-notice strong{color:var(–accent);}

.products-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(310px,1fr));gap:2px;max-width:1100px;margin:0 auto;}
.product-card{background:var(–card);border:1px solid var(–border);overflow:hidden;transition:transform 0.25s,border-color 0.25s;}
.product-card:hover{transform:translateY(-4px);border-color:var(–red);}
.product-img{width:100%;height:320px;overflow:hidden;position:relative;}
.product-img img{width:100%;height:100%;object-fit:cover;object-position:center top;transition:transform 0.4s;}
.product-card:hover .product-img img{transform:scale(1.04);}
.product-badge{position:absolute;top:14px;left:14px;padding:5px 12px;font-family:“Barlow Condensed”,sans-serif;font-weight:900;font-size:0.65rem;letter-spacing:2px;text-transform:uppercase;}
.badge-hot{background:var(–red);color:#fff;}
.badge-preorder{background:var(–accent);color:var(–black);}
.badge-limited{background:#444;color:#fff;}
.product-info{padding:22px;}
.product-name{font-family:“Barlow Condensed”,sans-serif;font-weight:700;font-size:1.1rem;letter-spacing:1px;text-transform:uppercase;margin-bottom:5px;}
.product-desc{font-size:0.8rem;color:var(–muted);margin-bottom:4px;line-height:1.5;}
.preorder-note{font-size:0.75rem;color:var(–accent);margin-bottom:12px;font-style:italic;}
.product-price{font-family:“Bebas Neue”,cursive;font-size:1.8rem;color:var(–red);letter-spacing:1px;margin-bottom:14px;}
.product-price small{font-size:0.8rem;color:var(–muted);font-family:“Barlow”,sans-serif;margin-left:4px;}
.size-select,.color-select{width:100%;background:#1e1e1e;color:var(–white);border:1px solid var(–border);padding:10px 14px;font-family:“Barlow”,sans-serif;font-size:0.85rem;margin-bottom:10px;cursor:pointer;outline:none;appearance:none;background-image:url(“data:image/svg+xml,%3Csvg xmlns=‘http://www.w3.org/2000/svg’ width=‘12’ height=‘8’ viewBox=‘0 0 12 8’%3E%3Cpath d=‘M1 1l5 5 5-5’ stroke=’%23666’ stroke-width=‘1.5’ fill=‘none’/%3E%3C/svg%3E”);background-repeat:no-repeat;background-position:right 14px center;padding-right:36px;}
.size-select:focus,.color-select:focus{border-color:var(–red);}
.add-to-cart{width:100%;background:var(–red);color:#fff;border:none;padding:13px;font-family:“Barlow Condensed”,sans-serif;font-weight:900;font-size:0.9rem;letter-spacing:3px;text-transform:uppercase;cursor:pointer;transition:all 0.2s;margin-top:4px;}
.add-to-cart:hover{background:#e02222;}
.add-to-cart:active{transform:scale(0.98);}
.out-of-stock{width:100%;background:#1a1a1a;color:#444;border:1px solid #2a2a2a;padding:13px;font-family:“Barlow Condensed”,sans-serif;font-weight:700;font-size:0.85rem;letter-spacing:2px;text-transform:uppercase;cursor:not-allowed;margin-top:4px;}

/* GALLERY */
#gallery{background:var(–black);}
.gallery-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:4px;max-width:1100px;margin:0 auto;}
.gallery-img{overflow:hidden;border:1px solid var(–border);}
.gallery-img img{width:100%;height:100%;object-fit:cover;transition:transform 0.4s;}
.gallery-img:hover img{transform:scale(1.03);}

/* CART */
.cart-overlay{position:fixed;inset:0;background:rgba(0,0,0,0.75);z-index:1000;display:none;opacity:0;transition:opacity 0.3s;}
.cart-overlay.open{display:block;opacity:1;}
.cart-sidebar{position:fixed;top:0;right:-500px;width:100%;max-width:480px;height:100%;background:var(–dark);border-left:1px solid var(–border);z-index:1001;display:flex;flex-direction:column;transition:right 0.35s cubic-bezier(0.4,0,0.2,1);}
.cart-sidebar.open{right:0;}
.cart-header{display:flex;align-items:center;justify-content:space-between;padding:26px 26px 18px;border-bottom:1px solid var(–border);}
.cart-header h2{font-family:“Bebas Neue”,cursive;font-size:1.5rem;letter-spacing:3px;}
.close-cart{background:none;border:none;color:var(–muted);font-size:1.4rem;cursor:pointer;transition:color 0.2s;}
.close-cart:hover{color:var(–white);}
.cart-items{flex:1;overflow-y:auto;padding:18px 26px;}
.cart-item{display:flex;gap:14px;padding:14px 0;border-bottom:1px solid var(–border);}
.cart-item-thumb{width:65px;height:65px;background:#1a1a1a;border:1px solid var(–border);overflow:hidden;flex-shrink:0;}
.cart-item-thumb img{width:100%;height:100%;object-fit:cover;}
.cart-item-info{flex:1;}
.cart-item-name{font-family:“Barlow Condensed”,sans-serif;font-weight:700;font-size:0.9rem;text-transform:uppercase;}
.cart-item-meta{font-size:0.72rem;color:var(–muted);margin-top:3px;}
.cart-item-price{font-family:“Bebas Neue”,cursive;font-size:1.05rem;color:var(–red);margin-top:5px;}
.cart-item-remove{background:none;border:none;color:var(–muted);cursor:pointer;font-size:1rem;align-self:flex-start;transition:color 0.2s;}
.cart-item-remove:hover{color:#cc1f1f;}
.cart-empty{text-align:center;padding:60px 20px;font-size:0.9rem;color:var(–muted);}
.cart-empty-icon{font-size:3rem;margin-bottom:14px;opacity:0.3;}
.cart-footer{padding:22px 26px;border-top:1px solid var(–border);background:var(–card);}
.cart-subtotal{display:flex;justify-content:space-between;font-size:0.8rem;color:var(–muted);margin-bottom:6px;}
.cart-shipping-line{display:flex;justify-content:space-between;font-size:0.8rem;color:#aaa;margin-bottom:10px;padding-bottom:10px;border-bottom:1px solid var(–border);}
.cart-total{display:flex;justify-content:space-between;align-items:center;margin-bottom:18px;}
.cart-total-label{font-size:0.78rem;letter-spacing:2px;text-transform:uppercase;color:var(–muted);}
.cart-total-amount{font-family:“Bebas Neue”,cursive;font-size:2rem;color:var(–red);}
.checkout-btn{width:100%;background:var(–red);color:#fff;border:none;padding:15px;font-family:“Barlow Condensed”,sans-serif;font-weight:900;font-size:0.95rem;letter-spacing:3px;text-transform:uppercase;cursor:pointer;transition:all 0.2s;margin-bottom:8px;}
.checkout-btn:hover{background:#e02222;}

/* MODAL */
.modal-overlay{position:fixed;inset:0;background:rgba(0,0,0,0.88);z-index:2000;display:none;align-items:flex-start;justify-content:center;padding:20px;overflow-y:auto;}
.modal-overlay.open{display:flex;}
.modal{background:var(–dark);border:1px solid var(–border);width:100%;max-width:560px;padding:36px;position:relative;animation:fadeUp 0.3s ease both;margin:auto;}
.modal-close{position:absolute;top:18px;right:18px;background:none;border:none;color:var(–muted);font-size:1.3rem;cursor:pointer;transition:color 0.2s;}
.modal-close:hover{color:var(–white);}
.modal h2{font-family:“Bebas Neue”,cursive;font-size:1.9rem;letter-spacing:3px;margin-bottom:6px;}
.modal .sub{font-size:0.8rem;color:var(–muted);margin-bottom:24px;line-height:1.6;}
.form-group{margin-bottom:16px;}
.form-group label{display:block;font-size:0.7rem;letter-spacing:2px;text-transform:uppercase;color:var(–muted);margin-bottom:7px;}
.form-group input,.form-group select,.form-group textarea{width:100%;background:#1e1e1e;color:var(–white);border:1px solid var(–border);padding:11px 15px;font-family:“Barlow”,sans-serif;font-size:0.88rem;transition:border-color 0.2s;outline:none;}
.form-group input:focus,.form-group select:focus{border-color:var(–red);}
.form-row{display:grid;grid-template-columns:1fr 1fr;gap:12px;}
.order-summary-mini{background:#0e0e0e;border:1px solid var(–border);padding:14px;margin-bottom:18px;}
.order-summary-mini h4{font-family:“Barlow Condensed”,sans-serif;font-weight:700;font-size:0.75rem;letter-spacing:2px;text-transform:uppercase;color:var(–muted);margin-bottom:10px;}
.order-line{display:flex;justify-content:space-between;font-size:0.82rem;padding:4px 0;border-bottom:1px solid #1a1a1a;}
.order-line:last-child{border-bottom:none;padding-top:8px;margin-top:4px;}
.order-line.total-line{font-weight:600;color:var(–red);font-family:“Bebas Neue”,cursive;font-size:1rem;}
.stripe-notice{background:#0a0800;border:1px solid #2a2000;padding:12px 14px;font-size:0.76rem;color:#a08030;margin-bottom:18px;line-height:1.6;}
.stripe-notice strong{color:var(–accent);}
.submit-btn{width:100%;background:var(–red);color:#fff;border:none;padding:15px;font-family:“Barlow Condensed”,sans-serif;font-weight:900;font-size:0.95rem;letter-spacing:3px;text-transform:uppercase;cursor:pointer;transition:all 0.2s;margin-top:6px;}
.submit-btn:hover{background:#e02222;}

/* DONATE */
#donate{background:#0a0000;}
.donate-container{max-width:680px;margin:0 auto;text-align:center;}
.donate-sub{color:var(–muted);font-size:0.92rem;margin-bottom:36px;line-height:1.8;max-width:500px;margin-left:auto;margin-right:auto;}
.donate-sub strong{color:#ddd;}
.donate-amounts{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-bottom:20px;}
.donate-amount-btn{background:var(–card);color:var(–white);border:1px solid var(–border);padding:16px 8px;font-family:“Bebas Neue”,cursive;font-size:1.4rem;letter-spacing:1px;cursor:pointer;transition:all 0.2s;}
.donate-amount-btn:hover,.donate-amount-btn.active{background:var(–red);color:#fff;border-color:var(–red);}
.donate-custom{display:flex;gap:10px;margin-bottom:24px;}
.donate-custom input{flex:1;background:var(–card);color:var(–white);border:1px solid var(–border);padding:13px 15px;font-family:“Barlow”,sans-serif;font-size:1rem;outline:none;transition:border-color 0.2s;}
.donate-custom input:focus{border-color:var(–red);}
.donate-btn{width:100%;background:var(–red);color:#fff;border:none;padding:17px;font-family:“Barlow Condensed”,sans-serif;font-weight:900;font-size:1.05rem;letter-spacing:3px;text-transform:uppercase;cursor:pointer;transition:all 0.2s;}
.donate-btn:hover{background:#e02222;transform:translateY(-2px);}
.donate-trust{display:flex;justify-content:center;gap:24px;margin-top:24px;font-size:0.73rem;color:var(–muted);letter-spacing:1px;flex-wrap:wrap;}
.donate-trust span::before{content:“✓ “;color:var(–success);}
.impact-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-bottom:36px;text-align:left;}
.impact-card{background:var(–card);border:1px solid #1a0000;border-left:3px solid var(–red);padding:16px 18px;}
.impact-card h4{font-family:“Barlow Condensed”,sans-serif;font-weight:700;font-size:0.9rem;text-transform:uppercase;letter-spacing:1px;margin-bottom:6px;color:var(–red);}
.impact-card p{font-size:0.78rem;color:var(–muted);line-height:1.5;}

footer{background:#050505;border-top:1px solid var(–border);padding:44px 36px;text-align:center;}
.footer-logo{font-family:“Bebas Neue”,cursive;font-size:1.9rem;letter-spacing:4px;color:var(–red);margin-bottom:10px;}
.footer-tagline{font-size:0.78rem;color:var(–muted);letter-spacing:3px;margin-bottom:22px;text-transform:uppercase;}
.footer-copy{font-size:0.7rem;color:#2a2a2a;letter-spacing:1px;}

.toast{position:fixed;bottom:28px;left:50%;transform:translateX(-50%) translateY(100px);background:var(–red);color:#fff;padding:13px 26px;font-family:“Barlow Condensed”,sans-serif;font-weight:700;font-size:0.88rem;letter-spacing:2px;text-transform:uppercase;z-index:9999;transition:transform 0.3s cubic-bezier(0.4,0,0.2,1);white-space:nowrap;}
.toast.show{transform:translateX(-50%) translateY(0);}

@keyframes fadeUp{from{opacity:0;transform:translateY(20px);}to{opacity:1;transform:translateY(0);}}
@media(max-width:640px){nav{padding:13px 16px;}.nav-links{display:none;}section{padding:60px 18px;}.donate-amounts{grid-template-columns:repeat(2,1fr);}.form-row{grid-template-columns:1fr;}.gallery-grid{grid-template-columns:1fr;}.impact-grid{grid-template-columns:1fr;}.modal{padding:24px 16px;}}
</style>

</head>
<body>

<nav>
  <a class="nav-logo" href="#">
    <span>GRIND LEAD MOTIVATE</span>
  </a>
  <ul class="nav-links">
    <li><a href="#shop">Shop</a></li>
    <li><a href="#gallery">Gallery</a></li>
    <li><a href="#donate">Donate</a></li>
  </ul>
  <button class="cart-btn" onclick="toggleCart()">
    CART <span class="cart-count" id="cartCount">0</span>
  </button>
</nav>

<section class="hero">
  <div class="hero-bg" style="background-image:url('fire1.jpg');"></div>
  <div class="hero-overlay"></div>
  <div class="hero-content">
    <h1 class="hero-title">GRIND<br><span class="red">LEAD</span><br>MOTIVATE</h1>
    <p class="hero-sub">Official GLM Workout Shirts — wear your mentality. All proceeds fuel the community.</p>
    <div class="hero-cta">
      <a href="#shop" class="btn-red">Shop Now — $35</a>
      <a href="#donate" class="btn-outline">Support the Mission</a>
    </div>
  </div>
</section>

<div class="mission-bar">
  <p>
    <strong>🏫 100% of profits go back into the Asheville community.</strong><br>
    Every shirt you buy directly funds the <strong>GLM Back-to-School Backpack Giveaway</strong> and the <strong>GLM Scholarship Program</strong> — because we rise by lifting others.
  </p>
  <div class="mission-icons">
    <div class="mission-icon">🎒 Backpack Giveaway</div>
    <div class="mission-icon">🎓 GLM Scholarship</div>
    <div class="mission-icon">🏙️ Asheville Community</div>
  </div>
</div>

<section id="shop">
  <div class="shop-header">
    <div class="section-label">Official Collection</div>
    <h2 class="section-title">GET YOUR GEAR</h2>
    <div class="shipping-notice">
      📦 <strong>Shipping:</strong> $5.99 standard (5–7 days) · $12.99 priority (2–3 days) · Free on orders over $75<br>
      ⏳ <strong>Pre-order items</strong> ship in 2–3 weeks. In-stock items ship within 3–5 business days.
    </div>
  </div>
  <div class="products-grid" id="productsGrid"></div>
</section>

<section id="gallery">
  <div style="text-align:center">
    <div class="section-label">The Lineup</div>
    <h2 class="section-title">THE SHIRTS</h2>
  </div>
  <div class="gallery-grid">
    <div class="gallery-img" style="height:420px;"><img src="workout.jpg" alt="GLM Workout Shirts" loading="lazy"></div>
    <div class="gallery-img" style="height:420px;"><img src="fire2.jpg" alt="GLM Shirts" loading="lazy"></div>
    <div class="gallery-img" style="height:420px;"><img src="fire1.jpg" alt="GLM Shirts Fire" loading="lazy"></div>
  </div>
</section>

<section id="donate">
  <div class="donate-container">
    <div class="section-label">Give Back</div>
    <h2 class="section-title">FUEL THE<br>COMMUNITY</h2>

```
<div class="impact-grid">
  <div class="impact-card">
    <h4>🎒 Backpack Giveaway</h4>
    <p>Each year GLM provides fully stocked backpacks to students in the Asheville community heading back to school.</p>
  </div>
  <div class="impact-card">
    <h4>🎓 GLM Scholarship</h4>
    <p>We invest in Asheville's future by awarding scholarships to motivated young people chasing their dreams.</p>
  </div>
</div>

<p class="donate-sub">You don't have to buy a shirt to support the mission. <strong>Every dollar donated goes directly back into the Asheville community.</strong> No overhead. All heart.</p>

<div class="donate-amounts">
  <button class="donate-amount-btn" onclick="setDonation(5,this)">$5</button>
  <button class="donate-amount-btn active" onclick="setDonation(10,this)">$10</button>
  <button class="donate-amount-btn" onclick="setDonation(25,this)">$25</button>
  <button class="donate-amount-btn" onclick="setDonation(50,this)">$50</button>
</div>
<div class="donate-custom">
  <input type="number" id="customDonation" placeholder="Custom amount ($)" min="1" oninput="clearDonationBtns()">
</div>
<button class="donate-btn" onclick="openDonateModal()">❤️ Donate to the Community</button>
<div class="donate-trust">
  <span>Secure via Stripe</span>
  <span>Apple Pay Ready</span>
  <span>100% Goes to Community</span>
</div>
```

  </div>
</section>

<footer>
  <div class="footer-logo">GRIND LEAD MOTIVATE</div>
  <div class="footer-tagline">Asheville Strong · Built for the Community</div>
  <div class="footer-copy">© 2025 Grind Lead Motivate. All Rights Reserved.</div>
</footer>

<!-- CART SIDEBAR -->

<div class="cart-overlay" id="cartOverlay" onclick="toggleCart()"></div>
<div class="cart-sidebar" id="cartSidebar">
  <div class="cart-header">
    <h2>YOUR CART</h2>
    <button class="close-cart" onclick="toggleCart()">✕</button>
  </div>
  <div class="cart-items" id="cartItems">
    <div class="cart-empty"><div class="cart-empty-icon">🛒</div><p>Your cart is empty.<br>Add some gear above!</p></div>
  </div>
  <div class="cart-footer">
    <div class="cart-subtotal"><span>Subtotal</span><span id="cartSubtotal">$0.00</span></div>
    <div class="cart-shipping-line"><span>Shipping (Standard)</span><span id="cartShipping">$0.00</span></div>
    <div class="cart-total">
      <span class="cart-total-label">Total</span>
      <span class="cart-total-amount" id="cartTotal">$0.00</span>
    </div>
    <button class="checkout-btn" onclick="openCheckout()">CHECKOUT →</button>
  </div>
</div>

<!-- CHECKOUT MODAL -->

<div class="modal-overlay" id="checkoutModal">
  <div class="modal">
    <button class="modal-close" onclick="closeModal('checkoutModal')">✕</button>
    <h2>CHECKOUT</h2>
    <p class="sub">Secured by Stripe. Supports card, Apple Pay & Google Pay.</p>
    <div class="order-summary-mini" id="orderSummary"></div>
    <div class="stripe-notice">
      <strong>💡 Setup:</strong> Add your Stripe publishable key (see code comments) to accept live payments, Apple Pay & Google Pay instantly.
    </div>
    <div class="form-group"><label>Full Name</label><input type="text" id="co-name" placeholder="John Doe"></div>
    <div class="form-group"><label>Email</label><input type="email" id="co-email" placeholder="you@email.com"></div>
    <div class="form-group"><label>Phone (optional)</label><input type="tel" id="co-phone" placeholder="+1 (555) 000-0000"></div>
    <div class="form-group"><label>Shipping Address</label><input type="text" id="co-address" placeholder="123 Main St, Asheville, NC 28801"></div>
    <div class="form-row">
      <div class="form-group"><label>City</label><input type="text" id="co-city" placeholder="Asheville"></div>
      <div class="form-group"><label>ZIP Code</label><input type="text" id="co-zip" placeholder="28801"></div>
    </div>
    <div class="form-group">
      <label>Shipping Method</label>
      <select id="co-shipping" onchange="updateShippingChoice()">
        <option value="5.99">Standard — $5.99 (5–7 days)</option>
        <option value="12.99">Priority — $12.99 (2–3 days)</option>
      </select>
    </div>
    <div class="form-group">
      <label>Card Details</label>
      <div id="stripe-card-element" style="background:#1e1e1e;border:1px solid var(--border);padding:13px 15px;">
        <div style="color:var(--muted);font-size:0.8rem;font-style:italic;">Stripe card field loads when you connect your account.</div>
      </div>
    </div>
    <button class="submit-btn" onclick="submitOrder()">PLACE ORDER →</button>
  </div>
</div>

<!-- DONATE MODAL -->

<div class="modal-overlay" id="donateModal">
  <div class="modal">
    <button class="modal-close" onclick="closeModal('donateModal')">✕</button>
    <h2>DONATE</h2>
    <p class="sub">Your generosity directly funds the GLM Backpack Giveaway and Scholarship in Asheville.</p>
    <div class="order-summary-mini">
      <h4>Donation Summary</h4>
      <div class="order-line total-line"><span>Your Donation</span><span id="donateAmountDisplay">$10.00</span></div>
    </div>
    <div class="stripe-notice"><strong>💡 Setup:</strong> Connect Stripe to accept live donations with Apple Pay.</div>
    <div class="form-group"><label>Full Name</label><input type="text" id="don-name" placeholder="John Doe"></div>
    <div class="form-group"><label>Email</label><input type="email" id="don-email" placeholder="you@email.com"></div>
    <div class="form-group"><label>Message (optional)</label><textarea id="don-message" placeholder="Keep motivating the community!" style="background:#1e1e1e;color:var(--white);border:1px solid var(--border);padding:11px 15px;font-family:Barlow,sans-serif;font-size:0.88rem;outline:none;resize:vertical;min-height:70px;width:100%;"></textarea></div>
    <button class="submit-btn" style="background:var(--red);" onclick="submitDonation()">❤️ COMPLETE DONATION</button>
  </div>
</div>

<div class="toast" id="toast"></div>

<script>
const SHIRT_COLORS = {
  "Black/Red": { shirt:"#111", text:"#cc1f1f" },
  "Black/White": { shirt:"#111", text:"#f0f0f0" },
  "Black/Black": { shirt:"#111", text:"#333" },
  "Grey/White": { shirt:"#888", text:"#f0f0f0" },
  "White/Black": { shirt:"#f0f0f0", text:"#111" }
};

const PRODUCTS = [
  {
    id:1, name:"GLM Tee — S / M / L / 3XL", price:35,
    badge:"Pre-Order", badgeClass:"badge-preorder",
    desc:"S, M, L, and 3XL are available by pre-order. Made fresh for you — ships in 2–3 weeks.",
    preorderNote:"⏳ Pre-order — ships in 2–3 weeks",
    sizes:["S","M","L","3XL"],
    colors:["Black/Red","Black/White","Grey/White","White/Black","Black/Black"],
    imgKey:"workout"
  },
  {
    id:2, name:"GLM Tee — XL (In Stock)", price:35,
    badge:"In Stock", badgeClass:"badge-hot",
    desc:"XL is in stock and ready to ship! Available in Black/Red, Grey/White, Black/White, and White/Black. Ships in 3–5 business days.",
    preorderNote: null,
    sizes:["XL"],
    colors:["Black/Red","Grey/White","Black/White","White/Black"],
    imgKey:"fire2"
  },
  {
    id:3, name:"GLM Tee — XXL (In Stock)", price:35,
    badge:"In Stock", badgeClass:"badge-hot",
    desc:"XXL is in stock and ready to ship! Available in Grey/White, Black/Red, Black/White, and Black/Black. Ships in 3–5 business days.",
    preorderNote: null,
    sizes:["XXL"],
    colors:["Grey/White","Black/Red","Black/White","Black/Black"],
    imgKey:"fire1"
  }
];

const imgMap = {
  workout: "workout.jpg",
  inventory: "",
  fire1: "fire1.jpg",
  fire2: "fire2.jpg"
};

function renderProducts() {
  const grid = document.getElementById("productsGrid");
  grid.innerHTML = PRODUCTS.map(p => `
    <div class="product-card">
      <div class="product-img">
        <img src="${imgMap[p.imgKey]}" alt="${p.name}" loading="lazy">
        <div class="product-badge ${p.badgeClass}">${p.badge}</div>
      </div>
      <div class="product-info">
        <div class="product-name">${p.name}</div>
        <div class="product-desc">${p.desc}</div>
        ${p.preorderNote ? `<div class="preorder-note">${p.preorderNote}</div>` : ""}
        <div class="product-price">$${p.price}.00 <small>+ shipping</small></div>
        <select class="size-select" id="size-${p.id}">
          <option value="">Select Size</option>
          ${p.sizes.map(s=>`<option value="${s}">${s}</option>`).join("")}
        </select>
        <select class="color-select" id="color-${p.id}">
          <option value="">Select Color</option>
          ${p.colors.map(c=>`<option value="${c}">${c}</option>`).join("")}
        </select>
        <button class="add-to-cart" onclick="addToCart(${p.id})">ADD TO CART</button>
      </div>
    </div>
  `).join("");
}

let cart = [];
let donationAmount = 10;
let shippingCost = 5.99;

function addToCart(id) {
  const p = PRODUCTS.find(x=>x.id===id);
  const size = document.getElementById(`size-${id}`).value;
  const color = document.getElementById(`color-${id}`).value;
  if (!size) { showToast("Please select a size!"); return; }
  if (!color) { showToast("Please select a color!"); return; }
  const existing = cart.find(i=>i.id===id&&i.size===size&&i.color===color);
  if (existing) existing.qty++;
  else cart.push({...p, size, color, qty:1, cartId:Date.now()});
  updateCartUI();
  showToast(`${p.name} (${size}, ${color}) added! 🔥`);
}

function removeFromCart(cartId) {
  cart = cart.filter(i=>i.cartId!==cartId);
  updateCartUI();
}

function updateCartUI() {
  const count = cart.reduce((a,i)=>a+i.qty,0);
  const subtotal = cart.reduce((a,i)=>a+i.price*i.qty,0);
  const shipping = cart.length > 0 ? (subtotal >= 75 ? 0 : shippingCost) : 0;
  const total = subtotal + shipping;

  const countEl = document.getElementById("cartCount");
  countEl.textContent = count;
  countEl.style.display = count > 0 ? "flex" : "none";
  document.getElementById("cartSubtotal").textContent = `$${subtotal.toFixed(2)}`;
  document.getElementById("cartShipping").textContent = shipping === 0 ? "FREE" : `$${shipping.toFixed(2)}`;
  document.getElementById("cartTotal").textContent = `$${total.toFixed(2)}`;

  const itemsEl = document.getElementById("cartItems");
  if (cart.length === 0) {
    itemsEl.innerHTML = `<div class="cart-empty"><div class="cart-empty-icon">🛒</div><p>Your cart is empty.<br>Add some gear above!</p></div>`;
  } else {
    itemsEl.innerHTML = cart.map(item=>`
      <div class="cart-item">
        <div class="cart-item-thumb"><img src="${imgMap[item.imgKey]}" alt="${item.name}"></div>
        <div class="cart-item-info">
          <div class="cart-item-name">${item.name}</div>
          <div class="cart-item-meta">${item.color} · ${item.size} · Qty ${item.qty}</div>
          ${item.preorderNote ? `<div style="font-size:0.68rem;color:var(--accent);margin-top:3px;">${item.preorderNote}</div>` : ""}
          <div class="cart-item-price">$${(item.price*item.qty).toFixed(2)}</div>
        </div>
        <button class="cart-item-remove" onclick="removeFromCart(${item.cartId})">✕</button>
      </div>
    `).join("");
  }
}

function toggleCart() {
  document.getElementById("cartOverlay").classList.toggle("open");
  document.getElementById("cartSidebar").classList.toggle("open");
}

function updateShippingChoice() {
  shippingCost = parseFloat(document.getElementById("co-shipping").value);
  buildOrderSummary();
}

function buildOrderSummary() {
  const subtotal = cart.reduce((a,i)=>a+i.price*i.qty,0);
  const shipping = subtotal >= 75 ? 0 : shippingCost;
  const total = subtotal + shipping;
  const el = document.getElementById("orderSummary");
  el.innerHTML = `
    <h4>Order Summary</h4>
    ${cart.map(i=>`<div class="order-line"><span>${i.name} · ${i.size}, ${i.color} ×${i.qty}</span><span>$${(i.price*i.qty).toFixed(2)}</span></div>`).join("")}
    <div class="order-line"><span>Shipping</span><span>${shipping===0?"FREE":"$"+shipping.toFixed(2)}</span></div>
    <div class="order-line total-line"><span>Total</span><span>$${total.toFixed(2)}</span></div>
  `;
}

function openCheckout() {
  if (cart.length===0) { showToast("Your cart is empty!"); return; }
  buildOrderSummary();
  toggleCart();
  document.getElementById("checkoutModal").classList.add("open");
}

function closeModal(id) { document.getElementById(id).classList.remove("open"); }

function submitOrder() {
  const name = document.getElementById("co-name").value;
  const email = document.getElementById("co-email").value;
  const address = document.getElementById("co-address").value;
  if (!name || !email || !address) { showToast("Please fill in all required fields."); return; }
  showToast("✅ Order received! Check your email for confirmation.");
  closeModal("checkoutModal");
  cart = [];
  updateCartUI();
}

function setDonation(amount, btn) {
  donationAmount = amount;
  document.getElementById("customDonation").value = "";
  document.querySelectorAll(".donate-amount-btn").forEach(b=>b.classList.remove("active"));
  btn.classList.add("active");
}
function clearDonationBtns() {
  document.querySelectorAll(".donate-amount-btn").forEach(b=>b.classList.remove("active"));
  donationAmount = null;
}
function openDonateModal() {
  const custom = document.getElementById("customDonation").value;
  const amount = custom ? parseFloat(custom) : donationAmount;
  if (!amount || amount <= 0) { showToast("Please enter a donation amount."); return; }
  donationAmount = amount;
  document.getElementById("donateAmountDisplay").textContent = `$${parseFloat(amount).toFixed(2)}`;
  document.getElementById("donateModal").classList.add("open");
}
function submitDonation() {
  const name = document.getElementById("don-name").value;
  const email = document.getElementById("don-email").value;
  if (!name || !email) { showToast("Please enter your name and email."); return; }
  showToast(`❤️ Thank you ${name}! Your $${donationAmount.toFixed(2)} helps Asheville.`);
  closeModal("donateModal");
}

function showToast(msg) {
  const t = document.getElementById("toast");
  t.textContent = msg;
  t.classList.add("show");
  setTimeout(()=>t.classList.remove("show"), 3000);
}

renderProducts();

/* STRIPE SETUP:
   1. Sign up at https://stripe.com
   2. Get your Publishable Key from the Dashboard
   3. Uncomment below and paste your key:

const stripe = Stripe("YOUR_STRIPE_PUBLISHABLE_KEY");
const elements = stripe.elements();
const cardElement = elements.create("card", {
  style: { base: { color: "#f0f0f0", fontFamily: "Barlow, sans-serif", fontSize: "15px" } }
});
cardElement.mount("#stripe-card-element");

   Apple Pay & Google Pay activate automatically once Stripe is connected.
*/
</script>

</body>
</html>
