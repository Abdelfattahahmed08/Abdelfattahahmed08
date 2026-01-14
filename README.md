azq qa  § # 👋 Hi, I'm Abdelfattah Ahmed  
                                                                                                                                  
🎓 **Artificial Intelligence Student | Data Scientist**                                 
💡 Passionate about **Machine Learning**, **AI Development**, and **Problem Solving**      
🤝 Open to opportunities in **AI**, **Data Science**, and **Software Development**     
                              
### 🧠 About Me                 
- 🎯 Focused on building intelligent systems and data-driven solutions.  
- 📊 Interested in research, analytics, and the intersection between AI and real-world problems.  
- 🌱 Currently enhancing my knowledge in **Deep Learning** and **MLOps**.  
- 💬 Always eager to collaborate on innovative AI or data projects                          
                                                                                                      
### 🛠️ Skills & Tools                                           
- **Programming:** Python, R, SQL               
- **Data Science:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **AI & ML:** TensorFlow, PyTorch, OpenCV  
- **Tools:** Jupyter, VS Code, Git, GitHub  
- **Other Interests:** Data Visualization, Research, AI Ethics     
                       
### 🌐 Connect with Me
- [💼 LinkedIn](https://www.linkedin.com/in/abdelfattah-ahmed-88479a294/)  
- ✉️ Email: [contact.abdlfattahahmed@gmail.com](mailto:contact.abdlfattahahmed@gmail.com)

### 📈 GitHub Stats
![Abdelfattah's GitHub stats](https://github-readme-stats.vercel.app/api?username=Abdelfattahahmed08&show_icons=true&theme=default&hide_border=true)

### 🤖 Affiliations
- 👨‍💻 **IEEE Member**  
- 🎓 **Microsoft Learn Member**

⭐️ *“Strive not to be a success, but rather to be of value.” — Albert Einstein*


import random

def game():
    print("=" * 30)
    print("🎯 لعبة تخمين الرقم 🎯")
    print("=" * 30)

    secret_number = random.randint(1, 100)
    attempts = 0

    while True:
        guess = input("أدخل رقمًا بين 1 و 100 (أو q للخروج): ")

        if guess.lower() == "q":
            print("❌ خرجت من اللعبة")
            break

        if not guess.isdigit():
            print("⚠️ أدخل رقمًا صحيحًا فقط")
            continue

        guess = int(guess)
        attempts += 1

        if guess < secret_number:
            print("⬆️ الرقم أكبر")
        elif guess > secret_number:
            print("⬇️ الرقم أصغر")
        else:
            print("🎉 مبروك! الرقم صحيح")
            print(f"عدد المحاولات: {attempts}")
            break

    print("شكراً للعب ❤️")

game()

