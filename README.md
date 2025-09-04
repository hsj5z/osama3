
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>أسامة فون - متجر إلكتروني</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
:root {
  --primary: #2D5BFF;
  --secondary: #FF9F43;
  --dark: #1E2A4A;
  --light: #F8FAFC;
  --gray: #E2E8F0;
  --text: #2D3748;
  --text-light: #718096;
  --success: #48BB78;
  --danger: #E53E3E;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background: var(--light);
  color: var(--text);
  line-height: 1.6;
}

a {
  text-decoration: none;
  color: inherit;
}

.container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 15px;
}

/* Header Styles */
header {
  background: white;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  padding: 15px 0;
  position: sticky;
  top: 0;
  z-index: 100;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
  color: var(--primary);
}

nav ul {
  display: flex;
  list-style: none;
}

nav ul li {
  margin-left: 20px;
}

nav ul li a {
  font-weight: 500;
  transition: color 0.3s;
}

nav ul li a:hover {
  color: var(--primary);
}

.header-actions {
  display: flex;
  align-items: center;
  gap: 15px;
}

.cart-icon {
  position: relative;
  cursor: pointer;
}

.cart-count {
  position: absolute;
  top: -8px;
  right: -8px;
  background: var(--primary);
  color: white;
  font-size: 0.7rem;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.language-switch {
  cursor: pointer;
  padding: 5px 10px;
  border-radius: 4px;
  border: 1px solid var(--gray);
  font-size: 0.9rem;
}

/* Hero Section */
.hero {
  background: linear-gradient(rgba(45, 91, 255, 0.05), rgba(45, 91, 255, 0.1)), url('https://images.unsplash.com/photo-1510557880182-3d4d3cba35a5?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80');
  background-size: cover;
  background-position: center;
  padding: 80px 0;
  text-align: center;
  margin-bottom: 40px;
}

.hero h1 {
  font-size: 2.5rem;
  color: var(--dark);
  margin-bottom: 15px;
}

.hero p {
  font-size: 1.2rem;
  color: var(--text);
  max-width: 700px;
  margin: 0 auto;
}

/* Filter Section */
.filter-section {
  background: white;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
  margin-bottom: 30px;
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
  align-items: center;
}

.filter-group {
  display: flex;
  align-items: center;
  gap: 10px;
}

.filter-section input, 
.filter-section select {
  padding: 10px 15px;
  border: 1px solid var(--gray);
  border-radius: 4px;
  font-size: 0.9rem;
  outline: none;
  transition: border-color 0.3s;
}

.filter-section input:focus, 
.filter-section select:focus {
  border-color: var(--primary);
}

.filter-section label {
  font-weight: 500;
}

/* Products Grid */
.products {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 25px;
  margin-bottom: 50px;
}

.product {
  background: white;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 15px rgba(0,0,0,0.08);
  transition: transform 0.3s, box-shadow 0.3s;
}

.product:hover {
  transform: translateY(-5px);
  box-shadow: 0 6px 20px rgba(0,0,0,0.12);
}

.product-image {
  height: 200px;
  overflow: hidden;
  position: relative;
}

.product-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.5s;
}

.product:hover .product-image img {
  transform: scale(1.05);
}

.product-badge {
  position: absolute;
  top: 10px;
  left: 10px;
  background: var(--secondary);
  color: white;
  padding: 5px 10px;
  border-radius: 4px;
  font-size: 0.8rem;
  font-weight: 500;
}

.product-info {
  padding: 15px;
}

.product-brand {
  color: var(--primary);
  font-weight: 500;
  margin-bottom: 5px;
  font-size: 0.9rem;
}

.product-name {

مهمات, [9/5/2025 2:23 AM]
font-weight: 600;
  margin-bottom: 10px;
  font-size: 1.1rem;
  height: 50px;
  overflow: hidden;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}

.product-price {
  font-weight: bold;
  font-size: 1.2rem;
  color: var(--dark);
  margin-bottom: 15px;
}

.product-rating {
  display: flex;
  align-items: center;
  gap: 5px;
  margin-bottom: 15px;
}

.product-rating i {
  color: #FFD700;
  font-size: 0.9rem;
}

.product-actions {
  display: flex;
  justify-content: space-between;
}

.btn {
  padding: 8px 15px;
  border: none;
  border-radius: 4px;
  font-weight: 500;
  cursor: pointer;
  transition: background 0.3s;
}

.btn-primary {
  background: var(--primary);
  color: white;
}

.btn-primary:hover {
  background: #1a46e0;
}

.btn-icon {
  display: flex;
  align-items: center;
  gap: 5px;
}

/* Cart Sidebar */
.cart-sidebar {
  position: fixed;
  top: 0;
  right: -350px;
  width: 350px;
  height: 100%;
  background: white;
  box-shadow: -2px 0 15px rgba(0,0,0,0.1);
  overflow-y: auto;
  transition: right 0.4s ease;
  padding: 20px;
  z-index: 1000;
}

.cart-sidebar.active {
  right: 0;
}

.cart-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  padding-bottom: 15px;
  border-bottom: 1px solid var(--gray);
}

.cart-header h2 {
  color: var(--dark);
}

.close-cart {
  background: none;
  border: none;
  font-size: 1.5rem;
  cursor: pointer;
  color: var(--text-light);
}

.cart-item {
  display: flex;
  margin-bottom: 15px;
  padding-bottom: 15px;
  border-bottom: 1px solid var(--gray);
}

.cart-item-image {
  width: 70px;
  height: 70px;
  border-radius: 4px;
  overflow: hidden;
  margin-left: 10px;
}

.cart-item-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.cart-item-details {
  flex: 1;
}

.cart-item-name {
  font-weight: 500;
  margin-bottom: 5px;
}

.cart-item-price {
  color: var(--primary);
  font-weight: bold;
}

.cart-item-remove {
  background: none;
  border: none;
  color: var(--danger);
  cursor: pointer;
  font-size: 1.1rem;
}

.cart-total {
  margin-top: 20px;
  font-weight: bold;
  text-align: left;
  font-size: 1.2rem;
  padding-top: 15px;
  border-top: 2px solid var(--gray);
}

.checkout-btn {
  display: block;
  width: 100%;
  padding: 12px;
  background: var(--primary);
  color: white;
  border: none;
  border-radius: 4px;
  font-weight: bold;
  cursor: pointer;
  margin-top: 15px;
  transition: background 0.3s;
}

.checkout-btn:hover {
  background: #1a46e0;
}

.checkout-form {
  margin-top: 20px;
  display: none;
}

.checkout-form input {
  width: 100%;
  padding: 10px;
  margin: 8px 0;
  border: 1px solid var(--gray);
  border-radius: 4px;
}

.checkout-form button {
  width: 100%;
  padding: 12px;
  background: var(--success);
  color: white;
  border: none;
  border-radius: 4px;
  font-weight: bold;
  cursor: pointer;
  margin-top: 10px;
}

/* Footer */
footer {
  background: var(--dark);
  color: white;
  padding: 40px 0 20px;
}

.footer-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 30px;
  margin-bottom: 30px;
}

.footer-section h3 {
  font-size: 1.2rem;
  margin-bottom: 15px;
  position: relative;
  padding-bottom: 10px;
}

.footer-section h3::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 40px;
  height: 2px;
  background: var(--primary);
}

.footer-section ul {
  list-style: none;
}

.footer-section ul li {
  margin-bottom: 10px;
}

.footer-section ul li a {
  color: #CBD5E0;
  transition: color 0.3s;
}

.footer-section ul li a:hover {
  color: white;
}

.footer-section p {
  color: #CBD5E0;
  margin-bottom: 10px;
}

.social-icons {
  display: flex;
  gap: 15px;
  margin-top: 15px;
}

.social-icons a {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 36px;
  height: 36px;
  background: rgba(255,255,255,0.1);
  border-radius: 50%;
  transition: background 0.3s;
}

.social-icons a:hover {
  background: var(--primary);
}

.footer-bottom {
  text-align: center;

مهمات, [9/5/2025 2:23 AM]
padding-top: 20px;
  border-top: 1px solid rgba(255,255,255,0.1);
  color: #CBD5E0;
  font-size: 0.9rem;
}

/* Responsive Design */
@media (max-width: 768px) {
  .header-content {
    flex-direction: column;
    gap: 15px;
  }
  
  nav ul {
    justify-content: center;
    flex-wrap: wrap;
  }
  
  nav ul li {
    margin: 0 10px 10px;
  }
  
  .filter-section {
    flex-direction: column;
    align-items: stretch;
  }
  
  .filter-group {
    flex-direction: column;
    align-items: stretch;
  }
  
  .products {
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  }
  
  .cart-sidebar {
    width: 300px;
  }
}

@media (max-width: 480px) {
  .hero h1 {
    font-size: 2rem;
  }
  
  .hero p {
    font-size: 1rem;
  }
  
  .products {
    grid-template-columns: 1fr;
  }
  
  .cart-sidebar {
    width: 100%;
    right: -100%;
  }
}
</style>
</head>
<body>

<header>
  <div class="container">
    <div class="header-content">
      <div class="logo">أسامة فون</div>
      <nav>
        <ul>
          <li><a href="#">الرئيسية</a></li>
          <li><a href="#">الهواتف</a></li>
          <li><a href="#">السماعات</a></li>
          <li><a href="#">الإكسسوارات</a></li>
          <li><a href="#">عروض خاصة</a></li>
          <li><a href="#">اتصل بنا</a></li>
        </ul>
      </nav>
      <div class="header-actions">
        <div class="cart-icon" onclick="toggleCart()">
          <i class="fas fa-shopping-cart"></i>
          <span class="cart-count" id="cartCount">0</span>
        </div>
        <div class="language-switch" onclick="toggleLanguage()">
          <span>EN</span>
        </div>
      </div>
    </div>
  </div>
</header>

<section class="hero">
  <div class="container">
    <h1>اكتشف أحدث الهواتف الذكية</h1>
    <p>استمتع بأفضل العروض على أحدث الموديلات من أشهر الماركات العالمية</p>
  </div>
</section>

<div class="container">
  <section class="filter-section">
    <div class="filter-group">
      <input type="text" id="searchInput" placeholder="ابحث عن منتج..." onkeyup="filterProducts()">
    </div>
    <div class="filter-group">
      <label for="categoryFilter">الفئة:</label>
      <select id="categoryFilter" onchange="filterProducts()">
        <option value="all">الكل</option>
        <option value="phone">هواتف</option>
        <option value="earbuds">سماعات</option>
        <option value="accessory">إكسسوارات</option>
      </select>
    </div>
    <div class="filter-group">
      <label for="brandFilter">الماركة:</label>
      <select id="brandFilter" onchange="filterProducts()">
        <option value="all">الكل</option>
        <option value="samsung">سامسونج</option>
        <option value="apple">أبل</option>
        <option value="xiaomi">شاومي</option>
        <option value="huawei">هواوي</option>
      </select>
    </div>
    <div class="filter-group">
      <label for="sortFilter">الترتيب:</label>
      <select id="sortFilter" onchange="filterProducts()">
        <option value="default">افتراضي</option>
        <option value="price-asc">السعر: من الأقل للأعلى</option>
        <option value="price-desc">السعر: من الأعلى للأقل</option>
        <option value="bestseller">الأكثر مبيعاً</option>
        <option value="rating">الأعلى تقييماً</option>
      </select>
    </div>
  </section>

  <section class="products" id="productsContainer"></section>
</div>

<div id="cartSidebar" class="cart-sidebar">
  <div class="cart-header">
    <h2>سلة التسوق</h2>
    <button class="close-cart" onclick="toggleCart()">&times;</button>
  </div>
  <div id="cartItems"></div>
  <div class="cart-total" id="cartTotal">المجموع: 0 ر.س</div>
  <button class="checkout-btn" onclick="toggleCheckout()">إتمام الشراء</button>
  <form id="checkoutForm" class="checkout-form" onsubmit="submitOrder(event)">
    <input type="text" placeholder="الاسم الكامل" required>
    <input type="text" placeholder="العنوان" required>
    <input type="tel" placeholder="رقم الهاتف" required>
    <button type="submit">تأكيد الطلب</button>
  </form>
</div>

<footer>
  <div class="container">
    <div class="footer-content">

مهمات, [9/5/2025 2:23 AM]
<div class="footer-section">
        <h3>عن المتجر</h3>
        <p>متجر أسامة فون يوفر أحدث الهواتف الذكية والإلكترونيات بأفضل الأسعار وضمان الجودة.</p>
        <div class="social-icons">
          <a href="#"><i class="fab fa-facebook-f"></i></a>
          <a href="#"><i class="fab fa-twitter"></i></a>
          <a href="#"><i class="fab fa-instagram"></i></a>
          <a href="#"><i class="fab fa-youtube"></i></a>
        </div>
      </div>
      <div class="footer-section">
        <h3>روابط سريعة</h3>
        <ul>
          <li><a href="#">الرئيسية</a></li>
          <li><a href="#">منتجاتنا</a></li>
          <li><a href="#">العروض</a></li>
          <li><a href="#">الأسئلة الشائعة</a></li>
          <li><a href="#">اتصل بنا</a></li>
        </ul>
      </div>
      <div class="footer-section">
        <h3>خدمة العملاء</h3>
        <ul>
          <li><a href="#">سياسة الإرجاع</a></li>
          <li><a href="#">الشروط والأحكام</a></li>
          <li><a href="#">سياسة الخصوصية</a></li>
          <li><a href="#">طرق الدفع</a></li>
          <li><a href="#">تتبع الطلب</a></li>
        </ul>
      </div>
      <div class="footer-section">
        <h3>معلومات الاتصال</h3>
        <p><i class="fas fa-map-marker-alt"></i> الرياض، المملكة العربية السعودية</p>
        <p><i class="fas fa-phone"></i> +966 12 345 6789</p>
        <p><i class="fas fa-envelope"></i> info@osamaphone.com</p>
      </div>
    </div>
    <div class="footer-bottom">
      <p>© 2023 أسامة فون. جميع الحقوق محفوظة</p>
    </div>
  </div>
</footer>

<script>
// المنتجات
const products = [
  {id:1, nameAR:'هاتف سامسونج جالاكسي S22', nameEN:'Samsung Galaxy S22', price:2999, category:'phone', brand:'samsung', rating:4.8, bestseller:true, img:'https://images.unsplash.com/photo-1610945265064-0e34e5519bbf?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80'},
  {id:2, nameAR:'آيفون 14 برو', nameEN:'iPhone 14 Pro', price:4499, category:'phone', brand:'apple', rating:4.9, bestseller:true, img:'https://images.unsplash.com/photo-1675862360172-1d2c17ec61c6?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80'},
  {id:3, nameAR:'سماعات ايربودز برو', nameEN:'AirPods Pro', price:899, category:'earbuds', brand:'apple', rating:4.7, bestseller:true, img:'https://images.unsplash.com/photo-1606220588913-b3aacb4d2f46?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80'},
  {id:4, nameAR:'هاتف شاومي 12', nameEN:'Xiaomi 12', price:2499, category:'phone', brand:'xiaomi', rating:4.5, bestseller:false, img:'https://images.unsplash.com/photo-1651058006427-8de62dc5f5c3?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80'},
  {id:5, nameAR:'سماعات سامسونج بودز', nameEN:'Samsung Buds', price:599, category:'earbuds', brand:'samsung', rating:4.3, bestseller:false, img:'https://images.unsplash.com/photo-1590658268037-6bf12165a8df?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80'},
  {id:6, nameAR:'غطاء آيفون جلد', nameEN:'iPhone Leather Case', price:199, category:'accessory', brand:'apple', rating:4.2, bestseller:true, img:'https://images.unsplash.com/photo-1546868871-7041f2a55e12?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80'},
  {id:7, nameAR:'هاتف هواوي P50', nameEN:'Huawei P50', price:2799, category:'phone', brand:'huawei', rating:4.4, bestseller:false, img:'https://images.unsplash.com/photo-1598324789736-4862f39a30c1?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80'},
  {id:8, nameAR:'شاحن لاسلكي', nameEN:'Wireless Charger', price:149, category:'accessory', brand:'samsung', rating:4.1, bestseller:false, img:'https://images.unsplash.com/photo-1609091839311-d5365f2e0c5a?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80'}
];

let cart = [];
let lang = 'ar';

function renderProducts() {
  const container = document.getElementById('productsContainer');
  container.innerHTML = '';
  
  products.forEach(p => {
    const stars = getStarRating(p.rating);
    
    const div = document.createElement('div');
    div.className = 'product';
    div.dataset.category = p.category;
    div.dataset.brand = p.brand;
    div.dataset.price = p.price;
    div.dataset.bestseller = p.bestseller;
    div.dataset.rating = p.

مهمات, [9/5/2025 2:23 AM]
rating;
    
    div.innerHTML = `
      <div class="product-image">
        <img src="${p.img}" alt="${lang === 'ar' ? p.nameAR : p.nameEN}">
        ${p.bestseller ? '<div class="product-badge">الأكثر مبيعاً</div>' : ''}
      </div>
      <div class="product-info">
        <div class="product-brand">${getBrandName(p.brand)}</div>
        <h3 class="product-name">${lang === 'ar' ? p.nameAR : p.nameEN}</h3>
        <div class="product-rating">${stars}</div>
        <div class="product-price">${p.price} ر.س</div>
        <div class="product-actions">
          <button class="btn btn-primary btn-icon" onclick="addToCart(${p.id})">
            <i class="fas fa-shopping-cart"></i> أضف إلى السلة
          </button>
        </div>
      </div>
    `;
    
    container.appendChild(div);
  });
}

function getStarRating(rating) {
  let stars = '';
  const fullStars = Math.floor(rating);
  const hasHalfStar = rating % 1 >= 0.5;
  
  for (let i = 0; i < fullStars; i++) {
    stars += '<i class="fas fa-star"></i>';
  }
  
  if (hasHalfStar) {
    stars += '<i class="fas fa-star-half-alt"></i>';
  }
  
  const emptyStars = 5 - fullStars - (hasHalfStar ? 1 : 0);
  for (let i = 0; i < emptyStars; i++) {
    stars += '<i class="far fa-star"></i>';
  }
  
  return stars;
}

function getBrandName(brandKey) {
  const brands = {
    'samsung': { ar: 'سامسونج', en: 'Samsung' },
    'apple': { ar: 'أبل', en: 'Apple' },
    'xiaomi': { ar: 'شاومي', en: 'Xiaomi' },
    'huawei': { ar: 'هواوي', en: 'Huawei' }
  };
  
  return brands[brandKey] ? brands[brandKey][lang] : brandKey;
}

function filterProducts() {
  const search = document.getElementById('searchInput').value.toLowerCase();
  const category = document.getElementById('categoryFilter').value;
  const brand = document.getElementById('brandFilter').value;
  const sort = document.getElementById('sortFilter').value;
  
  let filtered = products.filter(p => {
    const name = lang === 'ar' ? p.nameAR.toLowerCase() : p.nameEN.toLowerCase();
    const matchesSearch = name.includes(search);
    const matchesCategory = category === 'all' ? true : p.category === category;
    const matchesBrand = brand === 'all' ? true : p.brand === brand;
    
    return matchesSearch && matchesCategory && matchesBrand;
  });
  
  if (sort === 'price-asc') filtered.sort((a, b) => a.price - b.price);
  if (sort === 'price-desc') filtered.sort((a, b) => b.price - a.price);
  if (sort === 'bestseller') filtered.sort((a, b) => b.bestseller - a.bestseller);
  if (sort === 'rating') filtered.sort((a, b) => b.rating - a.rating);
  
  const container = document.getElementById('productsContainer');
  container.innerHTML = '';
  
  filtered.forEach(p => {
    const stars = getStarRating(p.rating);
    
    const div = document.createElement('div');
    div.className = 'product';
    div.innerHTML = `
      <div class="product-image">
        <img src="${p.img}" alt="${lang === 'ar' ? p.nameAR : p.nameEN}">
        ${p.bestseller ? '<div class="product-badge">الأكثر مبيعاً</div>' : ''}
      </div>
      <div class="product-info">
        <div class="product-brand">${getBrandName(p.brand)}</div>
        <h3 class="product-name">${lang === 'ar' ? p.nameAR : p.nameEN}</h3>
        <div class="product-rating">${stars}</div>
        <div class="product-price">${p.price} ر.س</div>
        <div class="product-actions">
          <button class="btn btn-primary btn-icon" onclick="addToCart(${p.id})">
            <i class="fas fa-shopping-cart"></i> ${lang === 'ar' ? 'أضف إلى السلة' : 'Add to Cart'}
          </button>
        </div>
      </div>
    `;
    
    container.appendChild(div);
  });
}

function addToCart(productId) {
  const product = products.find(p => p.id === productId);
  if (product) {
    cart.push({
      id: product.id,
      name: lang === 'ar' ? product.nameAR : product.nameEN,
      price: product.price,
      img: product.img
    });
    updateCartUI();
    
    // إشعار بإضافة المنتج
    alert(`${lang === 'ar' ? 'تمت إضافة' : 'Added'} ${lang === 'ar' ? product.nameAR : product.

مهمات, [9/5/2025 2:23 AM]
nameEN} ${lang === 'ar' ? 'إلى السلة' : 'to cart'}`);
  }
}

function removeFromCart(index) {
  cart.splice(index, 1);
  updateCartUI();
}

function updateCartUI() {
  document.getElementById('cartCount').innerText = cart.length;
  const cartItems = document.getElementById('cartItems');
  const cartTotal = document.getElementById('cartTotal');
  
  cartItems.innerHTML = '';
  let total = 0;
  
  cart.forEach((item, index) => {
    total += item.price;
    cartItems.innerHTML += `
      <div class="cart-item">
        <div class="cart-item-image">
          <img src="${item.img}" alt="${item.name}">
        </div>
        <div class="cart-item-details">
          <div class="cart-item-name">${item.name}</div>
          <div class="cart-item-price">${item.price} ر.س</div>
        </div>
        <button class="cart-item-remove" onclick="removeFromCart(${index})">
          <i class="fas fa-trash"></i>
        </button>
      </div>
    `;
  });
  
  cartTotal.innerText = ${lang === 'ar' ? 'المجموع: ' : 'Total: '}${total} ر.س;
}

function toggleCart() {
  document.getElementById('cartSidebar').classList.toggle('active');
}

function toggleCheckout() {
  const form = document.getElementById('checkoutForm');
  form.style.display = form.style.display === 'block' ? 'none' : 'block';
}

function submitOrder(e) {
  e.preventDefault();
  const name = document.getElementById('checkoutForm').querySelectorAll('input')[0].value;
  const address = document.getElementById('checkoutForm').querySelectorAll('input')[1].value;
  const phone = document.getElementById('checkoutForm').querySelectorAll('input')[2].value;
  let total = 0;
  cart.forEach(item => total += item.price);

  // هنا يمكنك إضافة كود إرسال الطلب إلى الخادم
  alert(`${lang === 'ar' ? 'شكراً لك!' : 'Thank you!'} ${lang === 'ar' ? 'تم استلام طلبك وسنتواصل معك قريباً.' : 'Your order has been received and we will contact you soon.'}`);
  
  document.getElementById('checkoutForm').reset();
  document.getElementById('checkoutForm').style.display = 'none';
  cart = [];
  updateCartUI();
  toggleCart();
}

function toggleLanguage() {
  lang = lang === 'ar' ? 'en' : 'ar';
  document.documentElement.dir = lang === 'ar' ? 'rtl' : 'ltr';
  document.documentElement.lang = lang;
  
  // تحديث النصوص حسب اللغة
  document.querySelector('.logo').innerText = lang === 'ar' ? 'أسامة فون' : 'Osama Phone';
  document.querySelector('nav ul li:nth-child(1) a').innerText = lang === 'ar' ? 'الرئيسية' : 'Home';
  document.querySelector('nav ul li:nth-child(2) a').innerText = lang === 'ar' ? 'الهواتف' : 'Phones';
  document.querySelector('nav ul li:nth-child(3) a').innerText = lang === 'ar' ? 'السماعات' : 'Earbuds';
  document.querySelector('nav ul li:nth-child(4) a').innerText = lang === 'ar' ? 'الإكسسوارات' : 'Accessories';
  document.querySelector('nav ul li:nth-child(5) a').innerText = lang === 'ar' ? 'عروض خاصة' : 'Special Offers';
  document.querySelector('nav ul li:nth-child(6) a').innerText = lang === 'ar' ? 'اتصل بنا' : 'Contact Us';
  
  document.querySelector('.language-switch span').innerText = lang === 'ar' ? 'EN' : 'AR';
  
  document.querySelector('.hero h1').innerText = lang === 'ar' ? 'اكتشف أحدث الهواتف الذكية' : 'Discover the Latest Smartphones';
  document.querySelector('.hero p').innerText = lang === 'ar' ? 'استمتع بأفضل العروض على أحدث الموديلات من أشهر الماركات العالمية' : 'Enjoy the best offers on the latest models from the most famous global brands';
  
  document.getElementById('searchInput').placeholder = lang === 'ar' ? 'ابحث عن منتج...' : 'Search for a product...';
  document.querySelector('label[for="categoryFilter"]').innerText = lang === 'ar' ? 'الفئة:' : 'Category:';
  document.querySelector('label[for="brandFilter"]').innerText = lang === 'ar' ? 'الماركة:' : 'Brand:';
  document.querySelector('label[for="sortFilter"]').innerText = lang === 'ar' ? 'الترتيب:' : 'Sort:';
  
  document.querySelector('#categoryFilter option[value="all"]').innerText = lang === 'ar' ? 'الكل' : 'All';
  document.querySelector('#categoryFilter option[value="phone"]').

مهمات, [9/5/2025 2:23 AM]
innerText = lang === 'ar' ? 'هواتف' : 'Phones';
  document.querySelector('#categoryFilter option[value="earbuds"]').innerText = lang === 'ar' ? 'سماعات' : 'Earbuds';
  document.querySelector('#categoryFilter option[value="accessory"]').innerText = lang === 'ar' ? 'إكسسوارات' : 'Accessories';
  
  document.querySelector('#brandFilter option[value="all"]').innerText = lang === 'ar' ? 'الكل' : 'All';
  
  document.querySelector('#sortFilter option[value="default"]').innerText = lang === 'ar' ? 'افتراضي' : 'Default';
  document.querySelector('#sortFilter option[value="price-asc"]').innerText = lang === 'ar' ? 'السعر: من الأقل للأعلى' : 'Price: Low to High';
  document.querySelector('#sortFilter option[value="price-desc"]').innerText = lang === 'ar' ? 'السعر: من الأعلى للأقل' : 'Price: High to Low';
  document.querySelector('#sortFilter option[value="bestseller"]').innerText = lang === 'ar' ? 'الأكثر مبيعاً' : 'Bestseller';
  document.querySelector('#sortFilter option[value="rating"]').innerText = lang === 'ar' ? 'الأعلى تقييماً' : 'Highest Rated';
  
  document.querySelector('.cart-header h2').innerText = lang === 'ar' ? 'سلة التسوق' : 'Shopping Cart';
  document.querySelector('.checkout-btn').innerText = lang === 'ar' ? 'إتمام الشراء' : 'Checkout';
  
  document.querySelector('#checkoutForm input[type="text"]:nth-child(1)').placeholder = lang === 'ar' ? 'الاسم الكامل' : 'Full Name';
  document.querySelector('#checkoutForm input[type="text"]:nth-child(2)').placeholder = lang === 'ar' ? 'العنوان' : 'Address';
  document.querySelector('#checkoutForm input[type="tel"]').placeholder = lang === 'ar' ? 'رقم الهاتف' : 'Phone Number';
  document.querySelector('#checkoutForm button[type="submit"]').innerText = lang === 'ar' ? 'تأكيد الطلب' : 'Confirm Order';
  
  renderProducts();
  updateCartUI();
}

// تهيئة الصفحة عند التحميل
document.addEventListener('DOMContentLoaded', function() {
  renderProducts();
});
</script>

</body>
</html>
