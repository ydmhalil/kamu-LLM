# KamuLLM ‑ Türkçe Kamu Soru‑Cevap Modeli

KamuLLM, **unsloth/llama‑3‑8b‑Instruct‑bnb‑4bit** tabanlı, Türkçe odaklı bir dil modelidir.  
Amacı: Vatandaşların kamu hizmetleri, yönetmelikler ve başvuru süreçleri hakkında
🚀 **doğru, güncel ve erişilebilir** cevaplar almasını sağlamak.

## 🔍 Veri Kümesi
| Kaynak | Ör. Sayısı | Açıklama |
|--------|-----------:|----------|
| Kurumsal SSS | 3950 | Resmî web sitelerinden kazındı, manuel temizlik yapıldı |
| Sentetik QA | 27728 | Mevzuat maddelerinden **Gemini 1.5 Flash** ile üretildi |
| **Toplam** | **31178** | CSV, `{"soru": "...", "cevap": "..."}` |

## ✨ Model Ayrıntıları
* unsloth tabanlı 4-bit LoRA (quantized adapter fine-tuning)
* 4‑bit quantization → inference ≈ 9 GB  

## ⏳ Sınırlar
* Çıktılar **hukuki danışmanlık yerini tutmaz**.  
* Mevzuat değişikliklerini yansıtmak için periyodik yeniden eğitime ihtiyaç duyar.  

> Katkı yapmak, veri hatası bildirmek veya entegrasyon (RAG/API) sorusu sormak için
[Issues](../../issues) kısmına yazın. 
