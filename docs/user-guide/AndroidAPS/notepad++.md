# Configuring Notepad++ for Home Assistant YAML

Using a local text editor like Notepad++ is a great way to manage your Home Assistant configuration files, but it handles formatting differently than Home Assistant itself. 

In Home Assistant, **literal Tab characters are forbidden**—it only accepts spaces. By default, Notepad++ often inserts a tab character when you press the Tab key, which can cause Home Assistant to throw configuration errors.

---

## 🛠️ How to Make Notepad++ Home Assistant Friendly

To configure Notepad++ so it automatically converts your tabs into the correct 2-space YAML format, follow these steps:

1. Open Notepad++ and go to **Settings > Preferences**.
2. Click on **Indentation** in the sidebar menu.
3. In the language dropdown list at the top, select **YAML** (making sure your YAML settings are targeted).
4. Under the replacement options, select **Space character(s)** (this acts as "Replace by space").
5. Change the **Indent size** from `4` to `2`.
6. Ensure that **Tab character** is **NOT** selected.

Once you apply these settings, pressing the Tab key in Notepad++ will automatically type **2 real spaces** instead of a tab character, keeping your code cleanly aligned and ready for Home Assistant!