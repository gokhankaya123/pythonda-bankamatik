while True:
    a = int(input("Paranız: "))
    b = int(input("Lütfen bir işlem seçiniz\n\n1- Bakiye sorgulama\n2- Para yatırma\n3- Para çekme\n4- Çıkış\nSeçiminiz: "))
    
    if b == 1:
        print("Anlık bakiyeniz:", a)
    
    elif b == 2:
        c = int(input("Ne kadar para yatırmak istersiniz: "))
        a += c
        print("Yeni bakiyeniz:", a)
    
    elif b == 3:
        d = int(input("Ne kadar para çekmek istersiniz: "))
        if d <= a:
            a -= d
            print("Anlık bakiyeniz:", a)
        else:
            print("Hesabınızda o kadar bakiye yok.")
    
    elif b == 4:
        print("Görüşürüz.")
        break
    
    else:
        print("Geçersiz bir seçim yaptınız, lütfen tekrar deneyin.")
