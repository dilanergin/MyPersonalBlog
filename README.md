# MyPersonalBlog
Blog Web Application.

	Siteyi tasarlarken konu bağımsız çeşitli yazıların paylaşılabileceği bir blog tasarlamayı düşündüm.
Sitenin ismine ve logosuna uygun tonlarda bir tema seçilerek renkler ona göre ayarlanmıştır.Benzer siteler incelenerek bir blog sitesinde olması gereken özellikler araştırılarak uygulanmıştır.
Sitenin tamamında google font link kullanılmıştır.

Sitede kullanılan bazı kod örnekleri :

-> Örnek Css Kodu:

.btn-icon {
  width: 32px;
  height: 32px;
  display: grid;
  place-items: center;
  background: var(--bg-green);
  border-radius: var(--radius-circle);
  color: var(--white);
}
-“İlginizi Çekebilir” bölümünde kullanılar buton şekil,renk ve boyutları yukarıdaki gibi ayarlanmıştır.
- Sitenin tamamında birbiri ile uyumlu renk ve şekil kullanılmasına özen gösterilmiştir.

-> Örnek html kodu:

 
                        <div class="card-wrapper">
                          <div class="card-tag">
                            
                            <a href="#" class="span hover-2">#Movie</a>
                          </div>
      
                        </div>
      
                        <h3 class="headline headline-3">
                          <a href="#" class="card-title hover-2">
                            Tekrar tekrar izlenilesi...
                          </a>
                        </h3>
      
                        <div class="card-wrapper">
      
                          <div class="profile-card">
                            <img src="./assets/images/author3.png" width="48" height="48" loading="lazy" alt="Joseph"
                              class="profile-poster">
      
                            <div>
                              <p class="card-title">Emre Can</p>
      
                              <p class="card-subtitle">1 Oct 2022</p>
                            </div>
                          </div>

-“Dilan Öneriyor” bölümünde orijinal bir tasarım düşünülerek yazı başlığı, yazı ile ilgili etiketler, yazar fotoğrafı, yazar ismi ve yazıldığı tarih gibi özellikler eklenmiştir.
-Aynı mantıkla diğer bölümler yapılmıştır.

-> Örnek Javascript Kodu:
-const header = document.querySelector("[data-header]");
const backTopBtn = document.querySelector("[data-back-top-btn]");

window.addEventListener("scroll", () => {
  if (window.scrollY > 100) {
    header.classList.add("active");
    backTopBtn.classList.add("active");
  } else {
    header.classList.remove("active");
    backTopBtn.classList.remove("active");
  }
- Bu kod ile sayfanın en altından en üstüne dönmeyi sağlayan buton eklenmiştir.
- Bu kod benzer bir site uygulamasından hazır olarak alınıp, değerleri, şekli ve rengi site temasına göre değiştirilmiştir. 


-> Örnek jQuery Kodu:

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.3/jquery.min.js"></script>

    <script>
      $(document).ready(function () {
        $(".btn-primary").click(function () {
          alert("İletişim Bilgileriniz Alınmıştır.Teşekkürler");
        });
      });
    </script>

<script>
    $(document).ready(function () {
      $("input").focus(function () {
        $(this).css("background-color", "bg-white-green");
      });
      $("input").blur(function () {
        $(this).css("background-color", "bg-white-green");
      });
    });
- “Subscribe” butonlarına basıldığında kullanıcıya verilen geri dönüş yukarıdaki gibi sağlanmıştır.

-> Uygulama responsive yapıdadır. Mobil ve web olarak kullanılabilir.
