# Seri ve Paralel Bağlama

## 1. Seri Bağlamanın Özellikleri

Seri bağlı dirençlerde:

1. **Akım her dirençten aynıdır.**
2. Toplam gerilim, dirençler üzerindeki gerilimlerin toplamıdır.
3. Eşdeğer direnç, dirençlerin toplamıdır.
4. Devredeki dirençlerden biri koparsa devrenin tamamından akım geçmez.

---

### Seri Bağlantıda Akım

Seri devrede tek bir akım yolu vardır. Bu nedenle:

$$I = I_1 = I_2 = I_3$$

> [!important] Akılda Tut
> **Seride akım AYNI.**

---

### Seri Bağlantıda Gerilim

Toplam gerilim, dirençlerin üzerindeki gerilimlerin toplamıdır:

$$V_{toplam} = V_1 + V_2 + V_3$$

Ohm Yasası:

$$V_1 = I \cdot R_1 \qquad V_2 = I \cdot R_2$$

Bu nedenle büyük direnç üzerinde daha büyük gerilim düşümü oluşur.

**Gerilim Oranı**

İki direnç için:

$$\frac{V_1}{V_2} = \frac{R_1}{R_2}$$

> Seri bağlı dirençlerde gerilim, direnç değerleriyle doğru orantılıdır.

---

### Seri Bağlantının Eşdeğer Direnci

$$R_{eş} = R_1 + R_2 + R_3$$

**Örnek:**

$$R_1 = 2\,\Omega \qquad R_2 = 3\,\Omega$$

$$R_{eş} = 2 + 3 = 5\,\Omega$$

---

### Seri Bağlantının Genel Özelliği

Seri bağlantıda eşdeğer direnç, en büyük dirençten de büyüktür:

$$R_{eş} > R_{en\ büyük\ direnç}$$

**Örnek:**

$$R_1 = 4\,\Omega \qquad R_2 = 6\,\Omega \qquad R_{eş} = 10\,\Omega$$

Dolayısıyla: $10 > 6$

---

## 2. Paralel Bağlama

Dirençlerin aynı iki noktaya bağlanmasına **paralel bağlama** denir.

```
       ┌──[ R₁ ]──┐
───────┤           ├───────
       └──[ R₂ ]──┘
```

### Paralel Bağlamanın Özellikleri

Paralel bağlı dirençlerde:

1. **Her direnç üzerindeki gerilim aynıdır.**
2. Toplam akım, kollardaki akımların toplamıdır.
3. Eşdeğer direnç, en küçük dirençten daha küçüktür.
4. Kollardan biri devre dışı kalırsa diğer kollar çalışmaya devam edebilir.

---

### Paralel Bağlantıda Gerilim

Tüm dirençler aynı iki noktaya bağlı olduğu için:

$$V = V_1 = V_2 = V_3$$

> [!important] Akılda Tut
> **Paralelde gerilim AYNI.**

---

### Paralel Bağlantıda Akım

Toplam akım, kollardaki akımların toplamıdır:

$$I_{toplam} = I_1 + I_2 + I_3$$

Her kol için Ohm Yasası uygulanır:

$$I_1 = \frac{V}{R_1} \qquad I_2 = \frac{V}{R_2}$$

---

### Paralel Bağlantının Eşdeğer Direnci

İki direnç için:

$$\frac{1}{R_{eş}} = \frac{1}{R_1} + \frac{1}{R_2}$$

Buradan:

$$R_{eş} = \frac{R_1 \cdot R_2}{R_1 + R_2}$$

Bu formül, özellikle **iki paralel direnç** için hızlı hesaplama sağlar.

---

### Üç Paralel Direnç

Üç direnç paralel bağlandığında formül şu şekilde genişler:

$$\frac{1}{R_{eş}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$$

(Daha fazla direnç eklendikçe sağ taraftaki terimler aynı mantıkla artmaya devam eder.)

---

## 3. Paralel Bağlantının Önemli Özelliği

Paralel bağlı dirençlerin eşdeğer direnci, **en küçük dirençten daha küçüktür.**

**Örnek:**

$$R_1 = 6\,\Omega \qquad R_2 = 3\,\Omega$$

$$R_{eş} = \frac{6 \cdot 3}{6+3} = \frac{18}{9} = 2\,\Omega$$

Görüldüğü gibi: $2\,\Omega < 3\,\Omega < 6\,\Omega$

> [!important]
> Paralel bağlantıda eşdeğer direnç, **en küçük dirençten bile küçüktür.**

---

## 4. Seri ve Paralel Karşılaştırması

| Özellik | Seri | Paralel |
|---|---|---|
| Akım | Aynı | Kollara bölünür |
| Gerilim | Bölünür | Aynı |
| Eşdeğer direnç | Dirençlerin toplamı | En küçük dirençten küçük |
| Akım yolu | Tek yol | Birden fazla yol |
| Bir direnç koparsa | Devre kesilir | Diğer kollar çalışmaya devam eder |
| Formül | $R_{eş} = R_1 + R_2 + \dots$ | $\dfrac{1}{R_{eş}} = \dfrac{1}{R_1} + \dfrac{1}{R_2} + \dots$ |

---

## 5. Ezberleme Mantığı

> [!tip] Kısa Kural

**SERİ**

- Akım aynı: $I_1 = I_2 = I$
- Dirençler toplanır: $R_{eş} = R_1 + R_2$
- Gerilim bölünür: $V = V_1 + V_2$

**PARALEL**

- Gerilim aynı: $V_1 = V_2 = V$
- Akımlar toplanır: $I = I_1 + I_2$
- Ters dirençler toplanır: $\dfrac{1}{R_{eş}} = \dfrac{1}{R_1} + \dfrac{1}{R_2}$

---

## 6. Fiziksel Mantık

### Seri

Akımın geçebileceği **tek yol** vardır.

```
→ → → [R₁] → → → [R₂] → → →
```

Akım herhangi bir noktada kaybolmadığı için:

$$I_1 = I_2$$

Dirençler akımın karşısına art arda çıktığı için toplam direnç büyür:

$$R_{eş} = R_1 + R_2$$

### Paralel

Akımın geçebileceği **birden fazla yol** vardır.

```
             ┌──[R₁]──┐
→ → → ───────┤         ├──────→
             └──[R₂]──┘
                 ↓
              Akım bölünür
```

Akım kollara ayrılır:

$$I = I_1 + I_2$$

Daha fazla yol oluştuğu için devrenin toplam direnci azalır.
