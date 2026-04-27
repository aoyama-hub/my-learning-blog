# 📓 My Learning & Project Log

This is my professional blog and accountability journal. It uses **Quarto** to turn Jupyter Notebooks into a static website hosted on GitHub Pages.

---

## 🚀 The Execution Loop (How to Push)

Follow these steps every time you want to update your blog:

### 1. Work (The "System")
* Activate your environment: `mamba activate blog_310`
* Do your work in a Jupyter Notebook (`.ipynb`) inside the `posts/` folder.
* **Crucial:** Ensure the top cell is a **Raw** or **Markdown** cell with metadata:
    ```yaml
    ---
    title: "Post Title"
    date: "2026-04-27"
    categories: [ML, Business, Music]
    ---
    ```

### 2. Render (The "Translation")
Once your notebook is saved and you've run the cells you want to show:
* Open your terminal in this folder.
* Run: `quarto render`
* *Note: This updates the `docs/` folder with the new HTML files.*

### 3. Push (The "Publishing")
* Open **GitHub Desktop**.
* You will see a list of changes (mostly inside the `docs/` folder).
* Enter a summary of what you did (e.g., "Added post on vision models").
* Click **Commit to main**.
* Click **Push origin**.

---

## 🛠 Project Structure
* `_quarto.yml`: The main configuration (themes, navbar, site settings).
* `index.qmd`: The home page (automatically lists posts from the `posts/` folder).
* `posts/`: Where your raw `.ipynb` project files live.
* `docs/`: The "finished" website (GitHub Pages looks here to show your blog).

---

## 🔗 Links
* **Live Blog:** [https://aoyama-hub.github.io/my-learning-blog](https://aoyama-hub.github.io/my-learning-blog)
* **Digital Garden:** [https://aoyama-hub.github.io](https://aoyama-hub.github.io)