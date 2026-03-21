# Collama - Ollama Modellerini Colab Üzerinde Çalıştır

Collama, Ollama modellerini Google Colab üzerinde zahmetsizce çalıştırmak için hazırlanmış minimal ve pratik bir setup repo’sudur.

Localde GPU’su olmayanlar ya da hızlıca model test etmek isteyenler için direkt çalıştırılabilir bir ortam sunar.

## İçerik
- Colab üzerinde tek tıkla Ollama kurulumu
- Llama, Qwen, Deepseek, CodeLlama gibi modelleri çalıştırma
- LangChain entegrasyonu ile prompt → response pipeline
- Minimum setup, maksimum hız

## Kimler İçin?
- Local GPU’su olmayan geliştiriciler
- Hızlı prototipleme yapmak isteyenler
- LLM’leri test etmek isteyenler
- Agent / automation kurmak isteyenler

## Ne Yapabilirsin?
- Coding LLM’leri test edebilirsin
- Prompt engineering deneyleri yapabilirsin
- Basit AI tool’lar geliştirebilirsin
- LangChain + Ollama workflow kurabilirsin

## Hızlı Başlangıç

Colab’da aç ve çalıştır:

https://colab.research.google.com/github/0x1881/collama/blob/main/Ollama_Setup.ipynb

Cloudflare Tunnel ile dışarıya bağlantı vererek çalıştırma:

Gereklilik:
- Cloudflare hesabı
- Cloudflare'e bağlı domain

Adımlar:
- Bu linkten https://one.dash.cloudflare.com/ Cloudflare Zero Trust paneline giriş yap.
- Networks > Connectors > Create a tunnel > Cloudflared > Tünel ismi ver > Select your device’s operating system (Debian)
- En aşağıdaki "cloudflared tunnel run --token ***" kısmındaki yıldızlı olan belirttiğim tokeni kopyalayıp Colab'ta gizli anahtarlara CLOUFLARE_TOKEN isminde ekle.

https://colab.research.google.com/github/0x1881/collama/blob/main/Ollama_Setup_with_Cloudflare_Tunnel.ipynb


## Limitler
- Colab session ephemeral (restart → her şey gider)
- GPU süresi sınırlı
- Büyük modellerde RAM/GPU yetmeyebilir

## Not
Bu repo production için değil, hızlı dene-çalıştır mantığı içindir.

## Katkı

Bu repo katkılara açıktır. Eğer notebook’unuz Ollama kullanarak başkalarına bir şeyler öğretebilecek bir use-case çözüyorsa, pull request göndermekten çekinmeyin.

## Teşekkür

Bu proje, https://github.com/5aharsh/collama reposundan ilham alınarak geliştirilmiştir.  
Orijinal fikir ve çalışma için proje sahibine teşekkür ederiz.
