FontDialog Example (C# WinForms)

A simple and practical Windows Forms application that demonstrates how to use the FontDialog component with "ShowColor = true" to let users select both font and text color for a TextBox.

---

📌 Overview

This project allows the user to:

- Open a Font Dialog
- Choose a custom font
- Pick any color for the text
- Apply the selected settings directly to a TextBox

This example is great for beginners who want to learn how to work with dialogs in Windows Forms.

---

⭐ Features

- ✔️ Change font style, size, and family
- ✔️ Choose custom text color (enabled via "ShowColor = true")
- ✔️ Real-time application of chosen settings
- ✔️ Clean and easy-to-understand code
- ✔️ Fully WinForms-based — no external libraries required

---

📂 Code Snippet (Main Logic)

private void button1_Click(object sender, EventArgs e)
{
    FontDialog fontDialog = new FontDialog();
    fontDialog.ShowColor = true;

    if (fontDialog.ShowDialog() == DialogResult.OK)
    {
        textBox1.Font = fontDialog.Font;
        textBox1.ForeColor = fontDialog.Color;
    }
}

---

🛠 Requirements

To run this project, you need:

- Windows OS
- Visual Studio (recommended)
- .NET Framework / .NET 6+
- A WinForms project with:
   - A TextBox named "textBox1"
   - A Button named "button1"

---

🚀 How to Use

1. Open the project in Visual Studio
2. Place a TextBox and a Button on the form
3. Double-click the button to generate a "Click" event
4. Paste the logic shown above
5. Run the project
6. Click the button → select font + color → settings apply instantl.

       
ـ
🤝 Contributions

Feel free to open Issues or PRs if you want to:

- Improve the UI
- Apply font/color to multiple controls
- Add save/load settings
- Extend the example further

---

⭐ If You Like This Project

Please consider giving the repository a star ⭐ to support development!
