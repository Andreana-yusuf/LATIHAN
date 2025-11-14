# sprint("Program Kategori Tinggi Badan")

while True:
    try:
        tinggi = float(input("Masukkan tinggi badan Anda (cm): "))
        if tinggi <= 0:
            print("Tinggi harus lebih dari 0. Coba lagi.")
            continue
        break
    except ValueError:
        print("Input harus berupa angka. Coba lagi.")

if tinggi < 150:
    kategori = "Pendek"
elif 150 <= tinggi < 170:
    kategori = "Normal"
else:
    kategori = "Tinggi"

print(f"Tinggi Anda {tinggi} cm dan Anda termasuk kategori: {kategori}.")
