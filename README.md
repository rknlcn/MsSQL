# MsSQL
İlişki Türleri

İster web ister windows uygulaması yapalım veri tabanı SQL Kullanırız

1.İlişkisel veri tabanı (RDBMS) (ilişkisel veri tabanı)
	Mantığı, küçük birimlere böl ve bölümler arası ilişkiler kur.
	örnek;
		-öğrenci
		-öğretmen
		-lab
		-ders
	bu üstteki tabloların ilişkileri SQL de (MsSQL, Oracle, PostgreSQL(bedava, TUBİTAK destekli) , MySQL)

2. NoSQL (ilişkisel olmayan veri tabanı)
	json yapısı(MongoDB, Cassandra vb.)
    

Normalizasyon Kuralları:
    • Efektif kullanmak için yapılır.
    • Veri Güvenilirliğini sağlamak için uygulanır.

    1. 1NF (1.Normalizasyon Kuralları):
        1. aynı sütunda birden fazla veri barındırılmamalıdır.
        2. Aynı tür bilgiyi barındıran farklı sütunlar olmamalı.
        3. Aynı verileri tekrar etmemek için tablo haline getir.

    2. 2NF (2.Normalizasyon Kuralları):
        1. 1NF i uygula
        2. Verilerin tekil olduğundan emin olmak için Primary Key yerleştir.
        3. Tablolar arasında ilişkili olan tablolar birleştirilir (foreign key ile).

    3. 3NF (3.Normalizasyon Kuralları):
        1. 2NF i uygula.
        2. Ara tablo oluştur.

Tablolar Arası İlişki Türleri
    1. Bire çok ilişki (1-n) one to many
    2. Çoka çok ilişki (n-n) many to many
    3. Bire bir ilişki (1-1) one to one