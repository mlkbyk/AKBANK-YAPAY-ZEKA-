# 🚇 Metro Ağı Uygulaması

Bu proje, bir metro ağı içinde en kısa ve en optimal rotaları bulmak için **BFS (Breadth-First Search)** ve **A* (A-Star)** algoritmalarını kullanmaktadır.  
Kullanıcı, başlangıç ve hedef istasyonları belirleyerek, en hızlı veya en kısa mesafeli rotayı hesaplayabilir.

## 🚀 Kurulum ve Çalıştırma

### Gereksinimler:
- Python 3.x  

### Kullanım:
1. Python dosyanızı çalıştırın:
   ```bash
   metro_simulation.py

## 📚 Kullanılan Algoritmalar

### 1️⃣ BFS (Breadth-First Search - Genişlik Öncelikli Arama)
- En kısa durak sayısını bulmak için kullanılır.
- Grafı seviyelere ayırarak katman katman arama yapar.
- **Kullanım Amacı:** İstasyon sayısını minimize eden rotayı bulmak.

### 2️⃣ A* (A-Star) Algoritması
- Daha optimize ve en kısa mesafeli yolu bulmak için kullanılır.
- **G(n) + H(n)** formülünü kullanır:  
  - **G(n)**: Başlangıç noktasından şu anki düğüme olan mesafe.  
  - **H(n)**: Şu anki düğümden hedefe olan tahmini mesafe (heuristic).  
- **Kullanım Amacı:** En kısa mesafeli yolu hesaplamak.

## 🔧 Kullanılan Kütüphaneler

### 📌 `heapq`
- Öncelikli kuyruk (Priority Queue) işlemleri için kullanılır.
- A* algoritmasında en düşük maliyetli düğümü seçmek için kullanılır.

### 📌 `collections.defaultdict`
- Varsayılan değer atanabilen bir sözlük türüdür.
- Metro ağını düğümler (istasyonlar) ve kenarlar (hatlar) şeklinde saklamak için kullanılır.

### 📌 `collections.deque`
- Çift uçlu kuyruk veri yapısıdır.
- BFS algoritmasında kuyruk işlemleri için kullanılır.

### 📌 `typing`
- Kodun daha okunabilir ve anlaşılır olması için tip belirleme amaçlı kullanılır.
- Örneğin, `Dict[str, List[str]]` gibi türleri tanımlamak için.

### 📌 `Optional`
- Bir değişkenin değer alabileceğini veya `None` olabileceğini belirtir.


