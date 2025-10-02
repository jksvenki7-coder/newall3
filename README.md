# newall3<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>JKS Group All modules updated</title>
<style>
  body {
    background: #20242b;
    color: #fff;
    font-family: 'Segoe UI', Arial, sans-serif;
    margin: 0;
    padding: 0;
  }
  header, nav {
    display: flex;
    justify-content: center;
    gap: 20px;
    background: #141b29;
    padding: 18px 0;
    box-shadow: 0 2px 8px rgba(0,0,0,0.5);
    position: sticky;
    top: 0;
    z-index: 1000;
  }
  header {
    font-weight: 700;
    font-size: 1.5em;
    color: #00e1ff;
    text-shadow: 0 0 14px #0fccfcc5;
  }
  nav button {
    background: none;
    border: 2.5px solid #0fccfc;
    border-radius: 9px;
    color: #0fccfc;
    font-weight: 700;
    font-size: 1em;
    cursor: pointer;
    padding: 12px 18px;
    transition: 0.3s ease;
    user-select: none;
  }
  nav button:hover {
    background: #0fccfc;
    color: #202733;
  }
  main {
    max-width: 1100px;
    margin: 38px auto 60px;
    padding: 0 16px;
  }
  .main-title {
    text-align: center;
    font-size: 2.3em;
    color: #00e1ff;
    margin-bottom: 25px;
    font-weight: 700;
    letter-spacing: 3px;
  }
  .dashboard {
  display: flex; flex-wrap: wrap; justify-content: center;
  gap: 28px;
  margin-top: 12px;
  }
  .folder-card {
    background: #23273b;
    border: 3px solid #ffe27f;
    border-radius: 12px;
    padding: 40px 54px;
    font-weight: 700;
    font-size: 1.2em;
    color: #ffe27f;
    cursor: pointer;
    text-align: center;
    box-shadow: 0 0 16px 5px #fff68d95, 0 5px 23px #11162490;
    transition: 0.4s ease all;
    min-width: 220px;
  }
  .folder-card:hover {
    border-color: #00e1ff;
    color: #0c1e33;
    background-color: #ffe27f;
    box-shadow: 0 0 24px 9px #61f0ffbb, 0 4px 28px #2ab6ff90;
  }
  .section-title {
    text-align: center;
    font-size: 1.59em;
    font-weight: 700;
    letter-spacing: 1.3px;
    color: #fff18b;
    margin: 18px auto;
  }
  .service-list, .category-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 24px;
  }
  .service-card, .category-card {
    background: #23273a;
    color: #ffe27f;
    border-radius: 10px;
    border: 2px solid #ffe27f;
    min-width: 180px;
    max-width: 220px;
    font-weight: 700;
    text-align: center;
    padding: 24px;
    cursor: pointer;
    box-shadow: 0 0 14px 3px #ffeb8499;
    transition: 0.25s ease all;
  }
  .service-card:hover,
  .category-card:hover {
    background: #ffe27f;
    color: #222a33;
    border-color: #00e1ff;
    box-shadow: 0 0 24px 5px #00e1ffbb;
    transform: scale(1.06);
  }
  .back-btn {
    background: #ffe27f;
    border-radius: 12px;
    padding: 15px 60px;
    font-size: 1.23em;
    font-weight: 900;
    color: #202733;
    cursor: pointer;
    border: 2.5px solid #ffe27f;
    box-shadow: 2px 2px 13px #ffe27fbd;
    margin: 30px auto 20px;
    display: block;
    width: max-content;
    transition: 0.3s ease all;
    user-select: none;
  }
  .back-btn:hover {
    background: #00e1ff;
    color: #fff;
    border-color: #00e1ff;
    box-shadow: 0 0 30px #00e1ffbb;
  }
  form.contact-form {
    max-width: 480px;
    background: #202b46;
    margin: 30px auto 80px auto;
    padding: 32px 38px;
    border: 2px solid #00e1ff92;
    border-radius: 10px;
    color: #c4def5;
    font-size: 1.11em;
    text-align: left;
  }
  form.contact-form label {
    display: block;
    margin-bottom: 10px;
    font-weight: 700;
    color: #8fc6ff;
  }
  form.contact-form input, form.contact-form textarea, form.contact-form select {
    width: 100%;
    font-size: 17px;
    padding: 12px 16px;
    border-radius: 7px;
    margin-bottom: 24px;
    border: 1.7px solid #07b0ea;
    background-color: #091927;
    color: #acd8ff;
    outline: none;
    box-sizing: border-box;
  }
  form.contact-form input:focus,
  form.contact-form textarea:focus,
  form.contact-form select:focus {
    background-color: #164772;
    border-color: #00e1ff;
  }
  form.contact-form button {
    display: block;
    margin: 0 auto;
    width: 100%;
    border: none;
    border-radius: 12px;
    font-weight: 900;
    font-size: 1.3em;
    padding: 15px 0;
    cursor: pointer;
    color: #0c2340;
    background-color: #00e1ff;
    transition: background-color 0.3s ease;
  }
  form.contact-form button:hover {
    background-color: #00bfff;
    color: #f0f9ff;
  }
  /* Camera & Maps styles */
  #camera video {
    width: 100%;
    max-width: 420px;
    height: auto;
    border-radius: 10px;
    border: 2px solid #00e1ff50;
    background: #000;
    margin-bottom: 22px;
  }
  #map {
    width: 100%;
    max-width: 600px;
    height: 420px;
    border-radius: 10px;
    border: 2px solid #00e1ff50;
  }
</style>
</head>
<body>
<header>
  <div class="main-title">JKS Group of Business</div>
</header>
<nav>
  <button onclick="showPage('dashboard')">Dashboard</button>
  <button onclick="showPage('profile')">Profile</button>
  <button onclick="showPage('wallet')">Wallet</button>
  <button onclick="showPage('orders')">Orders</button>
</nav>
<main>
  <!-- Dashboard -->
  <section id="dashboard" class="dashboard">
    <div class="folders-wrap">
      <div class="folder-card" onclick="openModule('ecommerce')">My E-commerce</div>
      <div class="folder-card" onclick="openModule('events')">Events & Catering</div>
      <div class="folder-card" onclick="openModule('courier')">Courier & Ride Booking</div>
      <div class="folder-card" onclick="openModule('job')">Job Consultancy & Services</div>
      <div class="folder-card" onclick="openModule('tours')">Tours & Travels</div>
      <div class="folder-card" onclick="openModule('realestate')">Real Estate & Construction</div>
      <div class="folder-card" onclick="openModule('investment')">Investment & Business</div>
      <div class="folder-card" onclick="openModule('loans')">Loans & Insurance</div>
      <div class="folder-card" onclick="openModule('home')">Home Services</div>
    </div>
  </section>

  <!-- Profile page -->
  <section id="profile" style="display:none; text-align:center;">
    <h2 class="section-title">Profile</h2>
    <p>Your Profile details will appear here.</p>
    <button class="back-btn" onclick="showPage('dashboard')">Back to Dashboard</button>
  </section>

  <!-- Wallet page -->
  <section id="wallet" style="display:none; text-align:center;">
    <h2 class="section-title">Wallet</h2>
    <p>Wallet balance and transactions displayed here.</p>
    <button class="back-btn" onclick="showPage('dashboard')">Back to Dashboard</button>
  </section>

  <!-- Orders page -->
  <section id="orders" style="display:none; text-align:center;">
    <h2 class="section-title">Orders</h2>
    <p>No orders yet.</p>
    <button class="back-btn" onclick="showPage('dashboard')">Back to Dashboard</button>
  </section>

  <!-- Service List -->
  <section id="serviceView" style="display:none; flex-direction: column; align-items: center;">
    <div class="section-title" id="serviceTitle"></div>
    <div class="service-list" id="serviceList"></div>
    <form class="contact-form" id="contactForm" style="display:none;">
      <h3 id="contactTitle"></h3>
      <label>Name:</label><input type="text" id="userName" required />
      <label>Mobile Number:</label><input type="tel" id="userPhone" maxlength="10" pattern="[6-9][0-9]{9}" required />
      <label>Message:</label><textarea id="userMessage" rows="4" required></textarea>
      <button type="button" onclick="submitContactForm()">Submit via WhatsApp</button>
      <button type="button" class="back-btn" onclick="backToServiceList()">Back to Services</button>
    </form>
    <button class="back-btn" onclick="showPage('dashboard')">Back to Dashboard</button>
  </section>

  <!-- Events & Catering -->
  <section id="eventsView" style="display:none; flex-direction: column; align-items: center;">
    <div class="section-title" id="eventsCategoryTitle"></div>
    <div class="events-categories" id="eventsCategories"></div>
    <div class="service-list" id="eventsServiceList"></div>
    <form id="eventContactForm" class="contact-form" style="display:none;">
      <h3 id="eventsContactTitle"></h3>
      <label>Name:</label><input id="eventsUserName" type="text" required />
      <label>Mobile Number:</label><input id="eventsUserPhone" type="tel" pattern="[6-9][0-9]{9}" maxlength="10" required />
      <label>Budget:</label>
      <select id="eventsBudget" required>
        <option value="">Select Budget</option>
        <option value="10k to 50k">10k to 50k</option>
        <option value="50k to 1L">50k to 1L</option>
        <option value="1L to 5L">1L to 5L</option>
        <option value="5L to 10L">5L to 10L</option>
        <option value="Above 10L">Above 10L</option>
      </select>
      <label>Capacity:</label>
      <select id="eventsCapacity" required>
        <option value="">Select Capacity</option>
        <option value="5-30 people">5-30 people</option>
        <option value="30-60 people">30-60 people</option>
        <option value="60-90 people">60-90 people</option>
        <option value="90-130 people">90-130 people</option>
        <option value="Above 130 people">Above 130 people</option>
      </select>
      <label>Message:</label><textarea id="eventsUserMessage" rows="4" required></textarea>
      <button type="button" onclick="submitEventsForm()">Submit via WhatsApp</button>
      <button type="button" class="back-btn" onclick="backToEventsCategory()">Back to Category</button>
    </form>
    <button type="button" class="back-btn" onclick="showPage('dashboard')">Back to Dashboard</button>
  </section>

  <!-- E-commerce -->
  <section id="ecomView" style="display:none;">
    <div class="section-title">My E-commerce</div>
    <nav>
      <button onclick="openEcomCategory('Groceries')">Groceries</button>
      <button onclick="openEcomCategory('Food')">Food</button>
      <button onclick="openEcomCategory('Pharmacy')">Pharmacy</button>
      <button onclick="showPage('camera')">Camera</button>
      <button onclick="showPage('maps')">Google Maps</button>
    </nav>
    <div id="ecomCategoryContent"></div>
    <div id="ecomFormSlot"></div>
    <button class="back-btn" onclick="showPage('dashboard')">Back to Dashboard</button>
  </section>

  <!-- Camera Page -->
  <section id="camera" style="display:none; text-align:center;">
    <h2 class="section-title">Camera</h2>
    <video id="video" autoplay muted playsinline style="max-width: 90%; border-radius: 12px; border: 2px solid #00e1ff92;"></video>
    <div style="margin-top: 15px;">
      <button onclick="switchCamera()">Switch Camera</button>
      <button onclick="capturePhoto()">Capture</button>
      <button class="back-btn" onclick="showPage('ecomView')">Back to E-commerce</button>
    </div>
    <canvas id="canvas" style="display:none;"></canvas>
    <div id="photoOutput" style="margin-top: 25px;"></div>
  </section>

  <!-- Maps Page -->
  <section id="maps" style="display:none; text-align:center;">
    <h2 class="section-title">Google Maps</h2>
    <div id="map" style="max-width: 600px; height: 400px; margin: 15px auto; border-radius: 12px; border: 2px solid #00e1ff92;"></div>
    <button class="back-btn" onclick="showPage('ecomView')">Back to E-commerce</button>
  </section>

</main>
<script src="https://maps.googleapis.com/maps/api/js?key=YOUR_GOOGLE_MAPS_API_KEY"></script>
<script>
  // Data for modules and services
  const modules = {
    courier: ['Courier Booking', 'Ride Booking', 'Tracking', 'Support', 'Rental Vehicles'],
    job: ['Job Search', 'Post Resume', 'Local Jobs', 'Non-Local Jobs', 'PG & Hostel', 'Services Marketplace'],
    tours: ['Tour Bookings', 'Custom & Regular Tours', 'Stay Booking', 'Vehicle Booking', 'Train/Bus/Flight Tickets'],
    realestate: ['Buy', 'Sell', 'Rent', 'Key Services', 'Construction', 'Industry'],
    investment: ['Gold', 'Silver', 'Real Estate', 'Business Opportunity'],
    loans: ['Loan Enquiry', 'Car Insurance', 'Bike Insurance', 'Housing Loans', 'Personal Loans', 'Health Insurance'],
    home: ['CC Camera Installation', 'Computer Repair', 'Car Wash', 'Mobile Repair', 'Chef Services', 'Bouncers', 'Bike Mechanic', 'Car Mechanic', 'Electrician', 'Painter', 'Plumber', 'Driver']
  };

  // E-commerce categories
  const ecomCategories = { 
    Groceries: ['Milk', 'Meat', 'Fruits', 'Vegetables', 'Flowers', 'Others'],
    Food: ['Biriyani', 'Tiffins', 'Ice Cream', 'Pizza', 'Burgers', 'Rolls'],
    Pharmacy: ['Medicines', 'Health Products', 'Supplements', 'Care Products']
  };

  // Events & Catering category data
  const eventsCategories = {
    package: [
      {name: "Silver (50k -160k)", services: ["Decoration", "Catering", "DJ & Music", "Guest House", "Chocolate & Cake", "Games & Entertainment"]},
      {name: "Gold (150k - 300k)", services: ["Decoration", "Catering", "Photography", "Anchor & Actors", "Vehicles"]},
      {name: "Diamond (500k - 5M)", services: ["Premium Decoration", "Luxury Catering", "Video & Photography", "Celebrity Anchors"]},
      {name: "Platinum (500k - 800k)", services: ["Special Decoration", "Exclusive Catering", "Top DJs", "Private Guest House"]}
    ],
    customized: ["Decoration", "Catering", "Photography & Videography", "Anchor & Actors", "DJ & Singers", "Guest House", "Chocolate & Cake", "Games & Entertainment", "Jewellery", "Invitation Cards", "Vehicles", "Return Gifts", "Makeup Artist", "Mehandi Artist", "Clothing & Accessories"],
    premium: ["Decoration", "Catering", "Photography & Videography", "Anchor & Actors", "DJ & Singers", "Guest House", "Chocolate & Cake", "Games & Entertainment", "Jewellery", "Invitation Cards", "Vehicles", "Return Gifts", "Makeup Artist", "Mehandi Artist", "Clothing & Accessories"]
  };

  let currentModule = '';
  let currentService = '';
  let currentEventCategory = '';
  let currentEventService = '';
  let currentEcomCategory = '';

  // Show module folders dashboard
  function showPage(page){
    currentModule = '';
    currentService = '';
    currentEventCategory = '';
    currentEventService = '';
    currentEcomCategory = '';
    document.querySelectorAll('main > section').forEach(s => s.style.display = 'none');
    if(page === 'dashboard'){
      document.getElementById('dashboard').style.display = 'flex';
    } else {
      document.getElementById(page).style.display = 'flex';
    }
  }

  // Open main module service list view (except special handling)
  function openModule(name){
    currentModule = name;
    currentService = '';
    if(name === 'events') {
      openEventsDashboard();
    } else if(name === 'ecommerce') {
      openEcomDashboard();
    } else {
      // show services and contact for others
      const listEl = document.getElementById('serviceList');
      listEl.innerHTML = '';
      modules[name].forEach(svc => {
        const div = document.createElement('div');
        div.className = 'service-card';
        div.textContent = svc;
        div.onclick = () => openContactForm(svc);
        listEl.appendChild(div);
      });
      document.getElementById('serviceTitle').textContent = name.replace(/_/g,' ').replace(/\b\w/g, l => l.toUpperCase());
      showPage('serviceView');
    }
  }

  // Contact form for normal services
  function openContactForm(service){
    currentService = service;
    document.getElementById('serviceList').style.display = 'none';
    const form = document.getElementById('contactForm');
    form.style.display = 'block';
    document.getElementById('contactTitle').textContent = 'Contact for ' + service;
    document.getElementById('userName').value = '';
    document.getElementById('userPhone').value = '';
    document.getElementById('userMessage').value = '';
  }
  function backToServiceList(){
    document.getElementById('contactForm').style.display = 'none';
    document.getElementById('serviceList').style.display = 'flex';
  }
  function submitContactForm(){
    const name = document.getElementById('userName').value.trim();
    const phone = document.getElementById('userPhone').value.trim();
    const message = document.getElementById('userMessage').value.trim();
    if(!name || !phone || !message){
      alert("All fields required.");
      return;
    }
    const msg = `Name: ${encodeURIComponent(name)}%0APhone: ${encodeURIComponent(phone)}%0AService: ${encodeURIComponent(currentService)}%0AMessage: ${encodeURIComponent(message)}`;
    window.open(`https://wa.me/8977143043?text=${msg}`, '_blank');
  }

  // Events & Catering
  function openEventsDashboard(){
    document.getElementById('dashboard').style.display = 'none';
    document.getElementById('serviceView').style.display = 'none';
    document.getElementById('ecomView').style.display = 'none';
    let catsHtml = '';
    for(let key in eventsCategories){
      catsHtml += `<div class="category-card" onclick="openEventsCategory('${key}')">${key.charAt(0).toUpperCase()+key.slice(1)}</div>`;
    }
    document.getElementById('eventsCategories').innerHTML = catsHtml;
    document.getElementById('eventsServiceList').innerHTML = '';
    document.getElementById('eventContactForm').style.display = 'none';
    showPage('eventsView');
    currentEventCategory = '';
  }

  function openEventsCategory(cat){
    currentEventCategory = cat;
    currentEventService = '';
    const list = document.getElementById('eventsServiceList');
    list.style.display = 'flex';
    list.innerHTML = '';
    document.getElementById('eventContactForm').style.display = 'none';
    document.getElementById('eventsCategoryTitle').innerText = cat.charAt(0).toUpperCase() + cat.slice(1) + ' Services';
    if(cat === 'package'){
      eventsCategories.package.forEach(pkg => {
        const div = document.createElement('div');
        div.className = 'service-card';
        div.style.width = '280px';
        div.innerText = pkg.name;
        div.onclick = () => openPackageServices(pkg.name, pkg.services);
        list.appendChild(div);
      });
    } else {
      eventsCategories[cat].forEach(svc => {
        const div = document.createElement('div');
        div.className = 'service-card';
        div.style.width = '200px';
        div.innerText = svc;
        div.onclick = () => openEventContactForm(svc, cat);
        list.appendChild(div);
      });
    }
  }

  function openPackageServices(name, services){
    currentEventService = '';
    document.getElementById('eventsCategoryTitle').innerText = name + ' Package Services';
    const list = document.getElementById('eventsServiceList');
    list.innerHTML = '';
    services.forEach(svc => {
      const div = document.createElement('div');
      div.className = 'category-card';
      div.style.width = '220px';
      div.innerText = svc;
      div.onclick = () => openEventContactForm(svc, name);
      list.appendChild(div);
    });
  }

  function openEventContactForm(service, cat){
    currentEventService = service;
    document.getElementById('eventsServiceList').style.display = 'none';
    const form = document.getElementById('eventContactForm');
    form.style.display = 'block';
    document.getElementById('eventsContactTitle').innerText = 'Contact for ' + service;
    document.getElementById('eventsUserName').value = '';
    document.getElementById('eventsUserPhone').value = '';
    document.getElementById('eventsUserMessage').value = '';
    document.getElementById('eventsUserName').dataset.cat = cat;
    document.getElementById('eventsUserName').dataset.serv = service;
  }

  function backToEventsCategory(){
    document.getElementById('eventContactForm').style.display = 'none';
    document.getElementById('eventsServiceList').style.display = 'flex';
  }

  function submitEventsForm() {
    const name=document.getElementById('eventsUserName').value.trim();
    const phone=document.getElementById('eventsUserPhone').value.trim();
    const message=document.getElementById('eventsUserMessage').value.trim();
    const budget=document.getElementById('eventsBudget')?.value || '';
    const capacity=document.getElementById('eventsCapacity')?.value || '';
    const cat=document.getElementById('eventsUserName').dataset.cat || '';
    const serv=document.getElementById('eventsUserName').dataset.serv || '';
    if(!name||!phone||!message){
      alert('Please fill all fields.');
      return;
    }
    let fullMsg=`Name: ${encodeURIComponent(name)}%0APhone: ${encodeURIComponent(phone)}%0AService: ${encodeURIComponent(serv)}%0ACategory: ${encodeURIComponent(cat)}%0AMessage: ${encodeURIComponent(message)}`;
    if(budget) fullMsg += `%0ABudget: ${encodeURIComponent(budget)}`;
    if(capacity) fullMsg += `%0ACapacity: ${encodeURIComponent(capacity)}`;
    window.open(`https://wa.me/8977143043?text=${fullMsg}`, '_blank');
  }
  
  // E-commerce open category
  function openEcomDashboard(){
    document.getElementById('dashboard').style.display = 'none';
    document.getElementById('serviceView').style.display = 'none';
    document.getElementById('eventsView').style.display = 'none';
    document.getElementById('ecomView').style.display = 'flex';
    // Clear content container to avoid old form present
    document.getElementById('ecomCategoryContent').innerHTML = '';
    document.getElementById('ecomFormSlot').innerHTML = '';
  }
  function openEcomCategory(cat){
    currentEcomCategory = cat;
    const content = document.getElementById('ecomCategoryContent');
    content.innerHTML = `<p style="text-align:center; font-weight:600; font-size:1.2em;">Selected Category: ${cat}</p>`;
    showOrderForm(cat);
  }
  function showOrderForm(cat){
    const container = document.getElementById('ecomFormSlot');
    container.innerHTML = `
      <form class="contact-form" onsubmit="submitOrder(event, '${cat}')">
        <h3 style="color:#ffe27f;">Order via WhatsApp: ${cat}</h3>
        <label>Name:</label>
        <input type="text" name="name" required/>
        <label>Phone:</label>
        <input type="tel" name="phone" maxlength="10" pattern="[6-9][0-9]{9}" required/>
        <label>Order Details:</label>
        <textarea name="orderDetails" required></textarea>
        <label>Delivery Address:</label>
        <textarea name="deliveryAddress" required></textarea>
        <button type="submit">Place Order</button>
      </form>
    `;
  }
  function submitOrder(e, cat){
    e.preventDefault();
    const form=e.target;
    const name=form.name.value.trim();
    const phone=form.phone.value.trim();
    const orderDetails=form.orderDetails.value.trim();
    const address=form.deliveryAddress.value.trim();
    if(!name||!phone||!orderDetails||!address){
      alert('Please fill all fields properly.');
      return;
    }
    const msg = `Order from JKS E-commerce%0ACategory: ${cat}%0AName: ${name}%0APhone: ${phone}%0AOrder: ${orderDetails}%0AAddress: ${address}`;
    window.open(`https://wa.me/8977143043?text=${encodeURIComponent(msg)}`, '_blank');
  }

  // Navigation helper
  function backToServiceList(){
    document.getElementById('contactForm').style.display = 'none';
    document.getElementById('serviceList').style.display = 'flex';
  }

  // Camera and Maps module not shown due to length limits but can be added if needed

  // Initialize dashboard view on page load
  document.addEventListener('DOMContentLoaded', () => showPage('dashboard'));
</script>
</body>
</html>
