1. Apa yang dimaksud dengan State, Action, dan Reward dalam Reinforcement Learning?
   State : adalah kondisi atau posisi yang sedang dihadapi oleh agen di dalam suatu lingkungan (environment). Pada kasus FrozenLake, setiap kotak pada peta merupakan sebuah state yang menunjukkan posisi agen.
   Action : adalah tindakan yang dapat dipilih oleh agen pada setiap state, seperti bergerak ke kiri, kanan, atas, atau bawah. Setelah melakukan suatu action, agen akan menerima Reward,
   Reward : aitu nilai umpan balik yang menunjukkan apakah tindakan yang dilakukan memberikan hasil yang baik atau tidak. Pada FrozenLake, agen memperoleh reward sebesar 1 jika berhasil mencapai tujuan (goal) dan reward 0 jika belum berhasil atau gagal mencapai tujuan.
2. Apa fungsi dari Learning Rate (α)?
   Rate (α) berfungsi untuk mengatur seberapa besar pengaruh pengalaman baru terhadap pembaruan nilai pada Q-Table. Nilai α yang besar membuat agen lebih cepat mempelajari informasi baru karena perubahan nilai Q lebih signifikan, sedangkan nilai α yang kecil membuat proses
   pembelajaran berlangsung lebih lambat tetapi lebih stabil.
3. Apa fungsi dari Discount Factor (γ)?
   Discount Factor (γ) berfungsi untuk menentukan seberapa penting reward yang akan diperoleh di masa depan dibandingkan dengan reward yang diterima saat ini. Nilai γ yang mendekati 1 membuat agen lebih mempertimbangkan keuntungan jangka panjang dalam menentukan tindakan,
   sedangkan nilai yang mendekati 0 membuat agen lebih fokus pada reward yang diperoleh secara langsung.
4. Mengapa digunakan metode Exploration dan Exploitation?
   Metode Exploration dan Exploitation digunakan agar agen dapat belajar secara optimal. Exploration memungkinkan agen mencoba berbagai aksi secara acak sehingga dapat menemukan jalur atau strategi baru yang mungkin lebih baik. Sementara itu, Exploitation membuat agen memilih
   aksi yang memiliki nilai Q tertinggi berdasarkan pengalaman yang telah dipelajari sebelumnya. Kombinasi kedua metode ini membantu agen memperoleh pengetahuan yang lebih lengkap pada awal pelatihan dan kemudian memanfaatkan pengetahuan tersebut untuk mengambil keputusan terbaik s
   etelah proses pembelajaran berlangsung.
5. Bagaimana perubahan nilai reward setelah training 2000 episode?
   Setelah proses training selama 2000 episode, nilai reward mengalami peningkatan dibandingkan dengan awal pelatihan. Pada episode-episode awal, reward masih rendah dan tidak stabil karena agen masih banyak melakukan exploration serta belum mengetahui jalur terbaik menuju tujuan.
   Seiring bertambahnya jumlah episode, nilai Q-Table terus diperbarui sehingga agen semakin mampu memilih tindakan yang optimal. Akibatnya, reward menjadi lebih tinggi dan lebih konsisten, yang menunjukkan bahwa agen telah berhasil mempelajari strategi terbaik untuk mencapai goal
   dengan lebih sering dan lebih efisien.
