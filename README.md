🍲 რეცეპტების აპლიკაცია
ეს არის Android აპლიკაცია, რომელიც საშუალებას აძლევს მომხმარებლებს მოიძიონ, დაათვალიერონ და ნახონ რეცეპტების დეტალური ინფორმაცია. აპლიკაცია იყენებს Firebase Authentication-ს ავტორიზაციისთვის და თანამედროვე Android არქიტექტურულ კომპონენტებს.
🧱 აპლიკაციის სტრუქტურა
MainActivity – აპლიკაციის მთავარი activity, რომელიც ამოწმებს მომხმარებლის ავტორიზაციის სტატუსს Firebase-ის მეშვეობით. იგი იყენებს Android Navigation Component-ს და გადადის შესაბამის ეკრანზე (LoginFragment ან HostFragment).

Fragments:
LoginFragment – შესვლის ფორმა
![image](https://github.com/user-attachments/assets/8dd302d4-6465-4c16-b310-15a08d3cd243)

RegisterFragment – რეგისტრაციის ფორმა
![image](https://github.com/user-attachments/assets/1a2c4e80-a15d-4f75-9684-434be7b7a768)

ForgotPasswordFragment – პაროლის აღდგენის ფორმა
![image](https://github.com/user-attachments/assets/cec04b3c-8e47-4467-814f-e5e8ec6baa7d)

HostFragment – ჰოსთ ფრაგმენტი, რომელიც შეიცავს აპლიკაციის მთავარ ინტერფეისს
![image](https://github.com/user-attachments/assets/54f51d8e-1a8a-4f66-8cf8-64eaa0e2acd2)
![image](https://github.com/user-attachments/assets/d4ec79e0-929f-4001-8963-ea12efdd04b7)
![image](https://github.com/user-attachments/assets/3c9ca339-25c2-47af-a380-f4ec59a57c87)

FavouriteFragment – ფავორიტი რეცეპტების სია
![image](https://github.com/user-attachments/assets/6258b6fd-5f98-4779-9095-f9a83bc24121)


🔄 მონაცემები და ბაზები
Firebase Authentication – მომხმარებელთა რეგისტრაცია და ავტორიზაცია.
SearchedRecipesInfo – ინტერნეტიდან წამოღებული რეცეპტების მონაცემები ინახება ამ მონაცემთა კლასში.


📦 Adapter-ები და ViewBinding
ყველა ფრაგმენტში გამოყენებულია RecyclerView შემდეგი ადაპტერებით:
HomeFragmentRecyclerAdapter – მთავარი გვერდის რეცეპტების სიისთვის
DetailFragmentRecyclerAdapter – დეტალური რეცეპტების ინფორმაციისთვის
FavouriteFragmentRecyclerAdapter – ფავორიტად მონიშნული რეცეპტებისთვის


ყველა ადაპტერი იყენებს ViewBinding-ს უსაფრთხო და ეფექტური UI ელემენტებთან კავშირისათვის.
✅ გამოყენებული ტექნოლოგიები
Kotlin
Android Jetpack (Fragments, Navigation Component, ViewModel)
Firebase Authentication
RecyclerView
ViewBinding


