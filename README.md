uçaklar = [
    [ "Wright Flyer", 48, "kalkış başarılı" ], 
    [ "Benoist 14", 93, "kalkış başarısız" ], 
    [ "Arado Ar79", 250, "kalkış başarısız" ],
    [ "Tusaş Hürkuş", 515, "kalkış başarılı", ], 
    [ "F-15E Strike Eagle" , 3062, "kalkış başarılı" ]
]

yolcu_uçakları = []
gösteri_uçakları = []
savaş_uçakları = []

for plane in uçaklar :
    isim, max_hız, durum = plane
    if max_hız >= 300 :
        savaş_uçakları.append(plane)
    elif 250 <= max_hız < 300 :
        gösteri_uçakları.append(plane)   
    else :
        yolcu_uçakları.append(plane)    

print( "savaş uçakları", savaş_uçakları )
print( "gösteri uçakları", gösteri_uçakları )
print( "yolcu uçakları", yolcu_uçakları )  

Kalkmayan_Uçaklar_Listesi = []
Kalkan_Uçaklar_Listesi = []

for plane in uçaklar :
    isim, max_hız, durum = plane 
    if durum == "kalkış başarılı" :
        Kalkan_Uçaklar_Listesi.append(plane)
    else :
        Kalkmayan_Uçaklar_Listesi.append(plane)    

print("Kalkan Uçaklar Listesi", Kalkan_Uçaklar_Listesi)
print("Kalkmayan Uçaklar Listesi", Kalkmayan_Uçaklar_Listesi)       

plane2 = ["Benoist 14, Arado Ar79"]
plane.extend(plane2)
print(plane)





