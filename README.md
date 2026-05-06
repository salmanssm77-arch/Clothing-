<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VELORÉ | Luxury Fashion</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

body {
  background: #0a0a0a;
  color: white;
  overflow-x: hidden;
}

/* NAVBAR */
header {
  position: fixed;
  width: 100%;
  padding: 20px 60px;
  display: flex;
  justify-content: space-between;
  backdrop-filter: blur(10px);
  background: rgba(0,0,0,0.3);
  z-index: 1000;
}

header h1 {
  letter-spacing: 3px;
}

nav a {
  margin: 0 15px;
  text-decoration: none;
  color: white;
  transition: 0.3s;
}

nav a:hover {
  color: #aaa;
}

/* HERO */
.hero {
  height: 100vh;
  position: relative;
}

.hero video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.hero-content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

.hero-content h2 {
  font-size: 70px;
  letter-spacing: 5px;
}

.hero-content button {
  margin-top: 20px;
  padding: 12px 30px;
  border: none;
  background: white;
  color: black;
  cursor: pointer;
  transition: 0.3s;
}

.hero-content button:hover {
  background: black;
  color: white;
}

/* SECTION */
.section {
  padding: 100px 60px;
}

.section h2 {
  text-align: center;
  margin-bottom: 50px;
  font-size: 40px;
}

/* COLLECTIONS */
.collections {
  display: flex;
  gap: 20px;
}

.collection {
  flex: 1;
  height: 500px;
  background-size: cover;
  position: relative;
  overflow: hidden;
}

.collection:hover {
  transform: scale(1.05);
}

.collection span {
  position: absolute;
  bottom: 20px;
  left: 20px;
  font-size: 28px;
}

/* PRODUCTS */
.products {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
}

.product {
  background: #111;
  padding: 15px;
  transition: 0.3s;
}

.product:hover {
  transform: translateY(-10px);
}

.product img {
  width: 100%;
  height: 300px;
  object-fit: cover;
}

.product button {
  width: 100%;
  padding: 10px;
  background: white;
  border: none;
  margin-top: 10px;
  cursor: pointer;
}

/* LOOKBOOK */
.lookbook {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}

.lookbook img {
  width: 100%;
  height: 400px;
  object-fit: cover;
  transition: 0.4s;
}

.lookbook img:hover {
  transform: scale(1.1);
}

/* INSTAGRAM */
.insta {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
}

.insta img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

/* FOOTER */
footer {
  text-align: center;
  padding: 40px;
  background: black;
}

/* RESPONSIVE */
@media(max-width: 900px){
  .products {
    grid-template-columns: repeat(2, 1fr);
  }

  .collections {
    flex-direction: column;
  }

  .lookbook {
    grid-template-columns: 1fr;
  }

  .insta {
    grid-template-columns: repeat(3, 1fr);
  }
}
</style>
</head>

<body>

<header>
  <h1>VELORÉ</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#">Shop</a>
    <a href="#">Lookbook</a>
    <a href="#">Contact</a>
  </nav>
</header>

<section class="hero">
  <video autoplay muted loop>
    <source src="https://cdn.coverr.co/videos/coverr-fashion-model-walking-5176/1080p.mp4" type="video/mp4">
  </video>

  <div class="hero-content">
    <h2>REDEFINE FASHION</h2>
    <button>Explore Collection</button>
  </div>
</section>

<section class="section">
  <h2>Collections</h2>
  <div class="collections">
    <div class="collection" style="background-image:url('https://images.unsplash.com/photo-1490481651871-ab68de25d43d')">
      <span>Summer</span>
    </div>
    <div class="collection" style="background-image:url('https://images.unsplash.com/photo-1523381210434-271e8be1f52b')">
      <span>Streetwear</span>
    </div>
    <div class="collection" style="background-image:url('https://images.unsplash.com/photo-1503342217505-b0a15ec3261c')">
      <span>Luxury</span>
    </div>
  </div>
</section>

<section class="section">
  <h2>Featured Drops</h2>
  <div class="products">

    <div class="product">
      <img src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab">
      <h3>Essential Tee</h3>
      <p>₹1,499</p>
      <button>Add to Cart</button>
    </div>

    <div class="product">
      <img src="https://images.unsplash.com/photo-1541099649105-f69ad21f3246">
      <h3>Denim Jacket</h3>
      <p>₹3,999</p>
      <button>Add to Cart</button>
    </div>

    <div class="product">
      <img src="https://images.unsplash.com/photo-1512436991641-6745cdb1723f">
      <h3>Minimal Hoodie</h3>
      <p>₹2,499</p>
      <button>Add to Cart</button>
    </div>

    <div class="product">
      <img src="https://images.unsplash.com/photo-1520975922284-9e0c7d4d7e66">
      <h3>Urban Pants</h3>
      <p>₹2,199</p>
      <button>Add to Cart</button>
    </div>

  </div>
</section>

<section class="section">
  <h2>Lookbook</h2>
  <div class="lookbook">
    <img src="https://images.unsplash.com/photo-1483985988355-763728e1935b">
    <img src="https://images.unsplash.com/photo-1503342217505-b0a15ec3261c">
    <img src="https://images.unsplash.com/photo-1495121605193-b116b5b09a14">
  </div>
</section>

<section class="section">
  <h2>From Instagram</h2>
  <div class="insta">
    <img src="https://images.unsplash.com/photo-1490481651871-ab68de25d43d">
    <img src="https://images.unsplash.com/photo-1523381210434-271e8be1f52b">
    <img src="https://images.unsplash.com/photo-1503342217505-b0a15ec3261c">
    <img src="https://images.unsplash.com/photo-1512436991641-6745cdb1723f">
    <img src="https://images.unsplash.com/photo-1520975922284-9e0c7d4d7e66">
    <img src="https://images.unsplash.com/photo-1483985988355-763728e1935b">
  </div>
</section>

<footer>
  <p>© 2026 VELORÉ — Luxury Redefined</p>
</footer>

</body>
</html>
