<!DOCTYPE html>
<html lang="ar">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>متجر عُمراء</title>

<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;700&display=swap" rel="stylesheet">

<style>

body{
margin:0;
font-family:'Cairo',sans-serif;
background:#E8C88E;
color:#222;
}

header{
background:#E8C88E;
padding:15px;
display:flex;
justify-content:space-between;
align-items:center;
}

.logo{
width:80px;
}

nav a{
margin:10px;
text-decoration:none;
color:#1c2b1c;
font-weight:bold;
}

.hero{
text-align:center;
padding:40px 20px;
}

.hero h1{
font-size:28px;
}

.btn{
background:#1c2b1c;
color:white;
padding:12px 20px;
border-radius:10px;
text-decoration:none;
}

.products{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(160px,1fr));
gap:20px;
padding:20px;
}

.card{
background:white;
border-radius:15px;
padding:10px;
text-align:center;
box-shadow:0 4px 10px rgba(0,0,0,0.1);
}

.card img{
width:100%;
border-radius:10px;
}

.card button{
margin-top:10px;
background:#1c2b1c;
color:white;
border:none;
padding:10px;
border-radius:8px;
}

.cart{
position:fixed;
bottom:20px;
right:20px;
background:#1c2b1c;
color:white;
padding:15px;
border-radius:50%;
font-size:20px;
}

footer{
text-align:center;
padding:20px;
margin-top:30px;
}

</style>

</head>


<body>

<header>

<img src="logo.png" class="logo">

<nav>
<a href="#home">الرئيسية</a>
<a href="#products">المنتجات</a>
<a href="#about">من نحن</a>
</nav>

</header>


<section class="hero" id="home">

<h1>مرحبا بكم في متجر عُمراء</h1>

<p>أفضل العطور والمنتجات المختارة بعناية</p>

<a class="btn" href="#products">تصفح المنتجات</a>

</section>


<section id="products">

<h2 style="text-align:center">المنتجات</h2>

<div class="products">

<div class="card">
<img src="https://images.unsplash.com/photo-1541643600914-78b084683601">
<h3>عطر فاخر</h3>
<p>20$</p>
<button onclick="order('عطر فاخر')">اطلب الآن</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1592945403244-b3fbafd7f539">
<h3>عطر نسائي</h3>
<p>25$</p>
<button onclick="order('عطر نسائي')">اطلب الآن</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1615634260167-c8cdede054de">
<h3>عطر رجالي</h3>
<p>30$</p>
<button onclick="order('عطر رجالي')">اطلب الآن</button>
</div>

</div>

</section>


<section id="about" style="padding:30px;text-align:center">

<h2>من نحن</h2>

<p>

متجر عُمراء متجر متخصص في بيع العطور والمنتجات المختارة
بعناية مع خدمة طلب سهلة وسريعة عبر واتساب.

</p>

</section>


<footer>

<p>© 2026 Omara Store</p>

</footer>


<div class="cart">🛒</div>


<script>

function order(product){

let number="967000000000"

let msg="مرحبا اريد طلب "+product

window.open("https://wa.me/"+number+"?text="+msg)

}

</script>

</body>

</html>
