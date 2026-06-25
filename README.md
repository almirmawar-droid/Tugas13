Apa yang dimaksud dengan State, Action, dan Reward dalam Reinforcement Learning?
State adalah kondisi atau posisi yang sedang dihadapi agent dalam lingkungan.
Action adalah tindakan yang dapat dipilih agent pada suatu state. 
Reward adalah nilai umpan balik yang diterima agent setelah melakukan suatu action. Reward digunakan untuk menilai apakah tindakan yang dilakukan baik atau buruk.
Pada FrozenLake:
State : posisi agent pada petak tertentu. 
Action : bergerak kiri, kanan, atas, atau bawah. 
Reward :1 jika mencapai tujuan (goal), dan 0 jika belum mencapai tujuan.

Apa fungsi dari Learning Rate (α)?
Learning Rate (α) berfungsi untuk mengatur seberapa besar informasi baru mempengaruhi nilai Q-Table yang sudah ada. Nilai α yang besar membuat agent belajar lebih cepat, sedangkan nilai α yang kecil membuat pembelajaran lebih stabil tetapi lebih lambat.

Apa fungsi dari Discount Factor (γ)?
Discount Factor (γ) digunakan untuk menentukan seberapa penting reward di masa depan dibandingkan reward saat ini. Semakin besar nilai γ, semakin agent mempertimbangkan keuntungan jangka panjang ketika memilih tindakan.

Mengapa digunakan metode Exploration dan Exploitation?
Exploration digunakan agar agent mencoba berbagai tindakan baru dan menemukan kemungkinan jalur yang lebih baik. 
Exploitation digunakan agar agent memanfaatkan pengalaman yang sudah dipelajari untuk memilih tindakan terbaik. 
Kedua metode ini diperlukan agar agent tidak hanya mencoba-coba terus, tetapi juga dapat menggunakan pengetahuan yang telah diperoleh untuk mencapai tujuan secara optimal.

Bagaimana perubahan nilai reward setelah training 2000 episode?
Setelah training selama 2000 episode, nilai reward cenderung meningkat dan menjadi lebih stabil. Hal ini menunjukkan bahwa agent telah mempelajari jalur terbaik menuju goal sehingga semakin sering berhasil menyelesaikan tugas dibandingkan pada awal proses training.


Tugas Lanjutan
Modifikasi program sehingga:
1.	Menggunakan environment Taxi-v3 Menampilkan rata-rata reward setiap 100 episode Membandingkan hasil training 100,1000, 2000, dan 5000 episode
alpha = 0.8       # learning rate
gamma = 0.95      # discount factor
epsilon = 1.0     # exploration rate

epsilon_decay = 0.995
min_epsilon = 0.01

episodes = 100
max_steps = 100
 100
<img width="1029" height="1078" alt="image" src="https://github.com/user-attachments/assets/388e9d29-b490-4425-90bb-dfc97ad1fe4b" />



alpha = 0.8       # learning rate
gamma = 0.95      # discount factor
epsilon = 1.0     # exploration rate

epsilon_decay = 0.995
min_epsilon = 0.01

episodes = 1000
max_steps = 100
<img width="1298" height="1005" alt="image" src="https://github.com/user-attachments/assets/ef6e314e-85ae-4d26-877b-7735ec088a3f" />


alpha = 0.8       # learning rate
gamma = 0.95      # discount factor
epsilon = 1.0     # exploration rate

epsilon_decay = 0.995
min_epsilon = 0.01

episodes = 2000
max_steps = 100
<img width="1349" height="986" alt="image" src="https://github.com/user-attachments/assets/401ee0cb-12dd-4ff5-ac7a-5c8f77d8be95" />

alpha = 0.8       # learning rate
gamma = 0.95      # discount factor
epsilon = 1.0     # exploration rate

epsilon_decay = 0.995
min_epsilon = 0.01

episodes = 5000
max_steps = 100
<img width="1349" height="986" alt="image" src="https://github.com/user-attachments/assets/4dad0ed8-c8d7-48d2-8358-6c8fcf016ed0" />






