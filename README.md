# Pieter-Theodorus-Handoko-Tugas-2
flappy_floppy bug Fix

# List Bug: 

Bug #1: _score di GameManager does not exist (line 66) [Very High Bug]

Fix => _ sebelum score di GameManager dihilangin karena "_score" tidak ada, yang ada "score"


Bug #2: _score di game manager merupakn int sedangkan untuk text di "scoretext" membutuhkan string (game manager line 67) [Very High Bug]

Fix => menambahkan "" + di sebelum score di GameManager untuk "forced to string" dan menghapus _ di sebelum score supaya dapat terbaca


Bug #3: tap controller.rigidbody hides inherited member 'Component.rigidbody' [Low Bug]

Fix => 'new' ditambahkan di script TapController line 23


Bug #4: pesawat langsung jatuh [Very High Bug]

Fix => script 'Tap Controller' di inspector game object 'plane' belum dicentang/diaktifkan


Bug #5: NullReference [Very High Bug]

Fix => menambahkan script "CountdownText.OnCountdownFinished += OnCountdownFinished" pada on void enable()


Bug #6: paralax yang berhenti saat game start [Very High Bug]

Fix => tanda negasi(!) sebelum gameover di script GameManager  line 28 dihilangkan


Bug #7: pesawat tidak mau naik / turun [Very High Bug]

Fix => pada script TapController line 69 terdapat Vector2.down, diganti Vector2.Up supaya pesawat dapat naik saat di tap


Bug #8: pesawat tidak mau collision [Very High Bug]

Fix => masalah terdapat pada tag di game object dan script, untuk pillar bawah belum di tag serta tag untuk deadzone pada script TapController kelebihan 's'


Bug #9: High Score yang tidak tersimpan [High Bug]

Fix => dibagian script GameManager line 60 terdapat "if (score < savedscore)" tanda lebih kecil dari (<) diganti tanda lebih besar dari (>)

 
