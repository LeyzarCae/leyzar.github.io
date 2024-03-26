<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Leyzar Warouw</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #a7a7a9, #cccccc); 
            color: #fff; 
        }
        header, footer {
            background-color: #a7a7a9;
            text-align: center;
            padding: 20px 0;
        }
        nav {
            background-color: #313131;
            text-align: center;
            padding: 10px 0;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 10px;
        }
        section {
            padding: 20px;
            display: none; 
        }
        .galery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }
        .galery img {
            width: 200px; 
            height: 200px;
            object-fit: cover; 
        }
        .blog-post {
            margin-bottom: 20px;
            border-bottom: 1px solid #ccc;
            padding-bottom: 20px;
        }
        .contact-form {
            max-width: 400px;
            margin: 0 auto;
        }
        .contact-form p {
            margin: 0;
        }
        .contact-form p span {
            font-weight: bold;
        }
    </style>
</head>
<body>

<header>
    <h1>Leyzar Warouw</h1>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#galery">Galery</a>
    <a href="#blog">Blog</a>
    <a href="#contact">Contact</a>
</nav>

<section id="home">
    <h2>Halaman Utama (Home)</h2>
    <h2>Hai, Nama saya Leyzar.</h2>
</section>

<section id="galery">
    <h2>Galeri (Galery)</h2>
    <div class="galery">
        <!-- Kumpulan foto-foto -->
        <img src="LW1.jpeg" alt="Foto 1">
        <img src="LW2.jpeg" alt="Foto 2">
        <img src="LW3.jpeg" alt="Foto 3">
        <img src="LW4.jpeg" alt="Foto 4">
        <img src="LW5.jpeg" alt="Foto 5">
        <img src="LW6.jpeg" alt="Foto 6">
    </div>
</section>

<section id="blog">
    <h2>Blog</h2>
    <!-- Artikel-artikel-->
    <div class="blog-post">
        <h3>Tawa Meningkatkan Kesehatan</h3>
        <p>Tawa bukan hanya menyenangkan, tetapi juga baik untuk kesehatan Anda. 
           Ketika Anda tertawa, tubuh Anda melepaskan endorfin, yang dapat mengurangi rasa sakit dan stres serta meningkatkan suasana hati. 
           Bahkan, beberapa penelitian menunjukkan bahwa tawa dapat meningkatkan fungsi kardiovaskular dan meningkatkan sistem kekebalan tubuh.</p>
    </div>
    <div class="blog-post">
        <h3>Tidur yang Cukup Meningkatkan Kreativitas</h3>
        <p>Tidur yang cukup sangat penting untuk kesehatan mental dan kreativitas. Saat Anda tidur, otak Anda mengonsolidasikan ingatan dan memproses informasi yang diterima sepanjang hari. 
            Studi menunjukkan bahwa kurang tidur dapat menghambat kemampuan kreatif dan kognitif seseorang. 
            Oleh karena itu, pastikan untuk memberikan prioritas yang cukup untuk tidur agar dapat meningkatkan kreativitas Anda.</p>
    </div>
    <div class="blog-post">
        <h3>Meditasi Mengurangi Stres dan Meningkatkan Konsentrasi</h3>
        <p>Meditasi adalah praktik kuno yang telah terbukti mengurangi stres dan meningkatkan konsentrasi. Dengan fokus pada pernapasan dan kesadaran saat ini, meditasi dapat membantu menenangkan pikiran dan mengurangi gejala kecemasan. 
            Bahkan, penelitian neurologis menunjukkan bahwa meditasi secara teratur dapat mengubah struktur otak untuk meningkatkan fungsi kognitif dan emosional. 
            Menambahkan sedikit meditasi ke dalam rutinitas harian Anda dapat membawa manfaat yang signifikan bagi kesejahteraan Anda.</p>
    </div>
</section>

<section id="contact">
    <h2>Kontak (Contact)</h2>
    <form class="contact-form" action="#" method="post">
        <p><span>Nama:</span>Leyzar Ferdinand Warouw</p>
        <p><span>Email:</span>leyzarwarouw026@student.unsrat.ac.id</p>
        <p><span>No Telepon:</span> 085298645915</p>
    </form>
</section>

<script>
    
    document.querySelectorAll('nav a').forEach(anchor => {
        anchor.addEventListener('click', function(e) {
            e.preventDefault();
           
            document.querySelectorAll('section').forEach(section => {
                section.style.display = 'none';
            });
            
            document.querySelector(this.getAttribute('href')).style.display = 'block';
        });
    });
</script>

</body>
</html>
