# Personalized Letter Generator ✉️
This Python script automatically generates personalized letters from a template. It replaces a placeholder (`[name]`) in the template letter with each name from a list and saves the completed letters in an output folder.

## 📂 Project Structure
Input/
 ├── Names/
 │    └── invited_names.txt
 └── Letters/
      └── starting_letter.txt
Output/
 └── ReadyToSend/
      └── letter_for_<name>.txt
main.py

## 🚀 How It Works
1. **Read names** from `invited_names.txt`.  
2. **Read the letter template** from `starting_letter.txt`.  
3. For each name:  
   - Replace the `[name]` placeholder with the actual name.  
   - Save the new letter in `./Output/ReadyToSend/`.  

## ▶️ Usage
1. Clone this repo:
   git clone https://github.com/your-username/letter-generator.git
   cd letter-generator

2. Make sure your folder structure matches the one above.  
   - Add names in `./Input/Names/invited_names.txt`  
   - Write your template in `./Input/Letters/starting_letter.txt` (use `[name]` where the name should go).  

3. Run the script:
   python main.py

4. Find personalized letters in `./Output/ReadyToSend/`.  

## 🛠 Example
**Template (`starting_letter.txt`)**
Dear [name],

You are invited to my birthday party this Saturday!

Best,
Chinmay

**Names (`invited_names.txt`)**
Rahul
Aisha
Priya

**Output**
- letter_for_Rahul.txt  
- letter_for_Aisha.txt  
- letter_for_Priya.txt  

## 📜 License
This project is licensed under the MIT License.  

## 🌟 Ideas to Extend
- Use CSV input with names + extra fields (e.g., address, event details).  
- Add command-line arguments for file paths.  
- Generate PDFs instead of `.txt` files.  
- Build a simple GUI with Tkinter/Streamlit.  
