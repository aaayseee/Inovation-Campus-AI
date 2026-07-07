# [Lab 2] Personal Branding Website with Vibe Coding

**Samsung Innovation Campus - Chapter 1: Introduction to Generative AI**

Bu proje, üretken yapay zeka araçları (Claude & Gemini) kullanılarak "Vibe Coding" metodolojisiyle uçtan uca tasarlanmış ve kodlanmış bir kişisel marka web sitesi çalışmasıdır.

---

## Step 1 & 3: Profile Definition and Website Generation
Yapay zekanın beni tanıyıp içerikleri oluşturması ve ardından HTML/CSS kodunu tek seferde yazması için aşağıdaki "Mega Prompt" kullanılmıştır.

**Kullanılan AI Aracı:** Claude
**Kullanılan Komut (Prompt):**
> Sen uzman bir Kişisel Marka Danışmanı ve Kıdemli Front-End Geliştiricisisin. Ekte sana özgeçmişimi (CV) iletiyorum. Bu CV'deki tüm akademik geçmişimi, teknik yeteneklerimi, projelerimi, başarılarımı ve sosyal becerilerimi derinlemesine analiz etmeni istiyorum.
>
> Bu analiz doğrultusunda "Personal Branding Website with Vibe Coding" ödevim için şu 3 adımı eksiksiz tamamla:
>
> **ADIM 1: DEFINE YOUR PERSONAL PROFILE**
> CV'mi analiz ederek web sitemde kullanılmak üzere modern, enerjik, profesyonel ve teknoloji odaklı bir dille şu üç bölümü yaz:
> - **Who I Am** (Kim olduğum, vizyonum, çok yönlülüğüm ve öne çıkan güçlü yanlarım)
> - **My Skills** (Teknik yeteneklerim, kullandığım araçlar, öne çıkan projelerim ve başarılarım)
> - **My Future Goal** (CV'mdeki gidişata uygun olarak kariyerimdeki gelecek hedeflerim ve vizyonum)
> *Not: İçerikleri yazarken SADECE CV'deki gerçeklere sadık kal, kesinlikle halüsinasyon yapma veya olmayan bir bilgi ekleme, ancak bunu bir hikaye anlatımı (storytelling) gibi etkileyici yap.*
>
> **ADIM 2: GENERATE YOUR IMAGE PROMPTS**
> Web sitemdeki bu 3 bölümün yanına koymak üzere yapay zeka görsel araçlarında kullanabileceğim; modern, profesyonel, teknolojik ve yaratıcı temalı 3 adet İngilizce görsel üretim komutu (Image Prompt) hazırla. Komutlar doğrudan metinleri görselleştirmeye yönelik olsun.
>
> **ADIM 3: BUILD YOUR PERSONAL WEBSITE**
> Yukarıdaki içerikleri ve görselleri birleştiren, tek bir HTML dosyası içinde çalışan, responsive (mobil uyumlu), son derece şık, temiz (clean UI) ve modern bir web sitesi kodu yaz. Tasarımda profesyonelliği vurgulayan modern bir renk paleti kullan. Görseller için `<img src="gorsel1.jpg">`, `gorsel2.jpg`, `gorsel3.jpg` yer tutucularını ekle. Tüm CSS kodlarını `<style>` etiketi içine göm ki tek dosyada anında çalıştırabileyim.

**Teknik entegrasyon notu:** Üretilen görseller `images/` alt klasörüne kaydedilip HTML içindeki `<img>` etiketleri `images/gorsel1.jpg`, `images/gorsel2.jpg`, `images/gorsel3.jpg` yollarını gösterecek şekilde güncellenmiştir. Site tek bir HTML dosyası + bir görsel klasörü olarak birlikte çalışacak şekilde teslim edilmiştir.

---

## Step 2: Image Generation
Sitenin görsel dünyasını oluşturmak için AI tarafından üretilen promptlar kullanılmış ve görseller projeye entegre edilmiştir.

* **gorsel1.jpg (Who I Am):** "An editorial double-exposure portrait blending a young engineer's profile with a glowing circuit-board and factory-floor blueprint overlay, deep navy and teal color palette, cinematic tech lighting, professional style, no text."

* **gorsel2.jpg (My Skills):** "An abstract 3D visualization of an optimization route network - glowing nodes connected by curved light-trails over a dark navy background, amber and teal accent lights, resembling a logistics/MILP graph, clean minimal tech aesthetic, no text."

* **gorsel3.jpg (My Future Goal):** "A forward-looking digital illustration of a horizon line made of ascending data bars transforming into a highway/road, dawn-toned amber gradient sky meeting deep navy, symbolizing career growth through AI-driven engineering, minimal futuristic style, no text."

**İterasyon:** İlk denemede "Who I Am" görseli jenerik bir AI yüzü ürettiği için kişisel markayı yeterince yansıtmıyordu. Bunun üzerine prompt'u kendi fotoğrafımı referans alacak şekilde revize ettim:

> "Using the uploaded photo as the reference for the face and likeness, create a professional double-exposure portrait: keep the person's real facial features clearly recognizable and unaltered, blended subtly with a faint circuit-board pattern and isometric factory-line blueprint on the hair/background side only - not over the face. Deep navy and teal color grading, soft cinematic lighting, editorial tech-portrait style, no text, no distortion of facial features."

Bu revizyon sonucunda yüz net ve tanınabilir kalırken, teknik overlay yalnızca arka plan/saç bölgesine taşındı - kişisel marka için çok daha güçlü bir sonuç elde edildi. Ayrıca üretilen görsellerin köşesinde kalan platform filigranları, Claude ile birlikte basit bir görüntü işleme scripti (komşu bölgeden doku klonlama) kullanılarak temizlendi.

---

## Step 4: Review and Improve 

Süreç boyunca birkaç somut iyileştirme turu yapıldı:

1. **Renk paleti ve tipografi:** Jenerik "AI tasarımı" kliselerinden (krem zemin + terracotta, ya da siyah zemin + neon yeşil) kaçınmak için koyu lacivert + amber + teal paleti ve `Space Grotesk` / `Inter` / `JetBrains Mono` yazı tipi kombinasyonu bilinçli olarak seçildi.
2. **İmza tasarım öğesi:** Hero bölümüne, RouteIQ/MILP projelerime doğrudan gönderme yapan, canlı canvas animasyonuyla çizilen bir "optimizasyon rota ağı" eklendi - dekoratif değil, içerikle doğrudan bağlantılı bir seçim.
3. **Görsel kalite kontrolü:** İlk üretilen portre görseli kişisel markayı yeterince yansıtmadığı için kendi fotoğrafımla yeniden üretildi; sonrasında üç görseldeki platform filigranları temizlendi.
4. **Tam entegrasyon:** Başlangıçta yalnızca iki bölümde görsel kullanılıyordu; üçüncü görsel (yol/ufuk illüstrasyonu) "My Future Goal" bölümüne eklenerek üç bölümün de görsel açıdan tutarlı ve tam olması sağlandı.

Sonuç olarak **Full-Stack AI Developer & Innovator** rolünü hedefleyen, **modern, dinamik ve son derece profesyonel** hissettiren bir site ortaya çıktı. AI'yı yalnızca ilk taslak için değil, **anlamsal düzen, renk kontrastı ve bölümlerin hikaye anlatımı tonunu** iyileştirmek için de iteratif olarak kullandım - bu da geleceğe dönük kariyer vizyonumu daha iyi yansıtmasını sağladı.