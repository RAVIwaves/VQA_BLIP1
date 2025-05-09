# VQA_BLIP1

**Visual Question Answering using BLIP and Hugging Face Transformers**

This project demonstrates how to perform Visual Question Answering (VQA) using the [Salesforce BLIP](https://huggingface.co/Salesforce/blip-vqa-base) model from Hugging Face's `transformers` library. You can input an image and ask natural language questions to receive intelligent answers from the model.

---

## 📁 Project Structure

```
VQA_BLIP1/
├── images/
│   └── cat.jpg             # Sample image used for 
├── main.ipynb              # Jupyter notebook running the VQ
├── requirements.txt        # Python dependencies
├── vqa.yml                 # Optional conda environment file
└── README.md               # Project documentation
```

---

## 🚀 How It Works

1. Load the pretrained `Salesforce/blip-vqa-base` model and processor.
2. Read the input image using PIL.
3. Ask natural language questions about the image.
4. BLIP generates answers using a vision-language transformer.
5. Output answers are printed in response to each question.

---

## 🧠 Sample Questions

- What is the cat doing?
- What color is the wall?
- Is the cat sitting or standing?

These questions are customizable — feel free to ask anything about the image or change the image.

---

## 🖥️ Setup Instructions

### 1. Clone the repository

```bash
git clone <repo-url>
cd VQA_BLIP1
```

### 2. Install dependencies

Using `pip`:

```bash
pip install -r requirements.txt
```

Or create a conda environment:

```bash
conda env create -f vqa.yml
conda activate vqa_blip
```

### 3. Run the notebook

Open `main.ipynb` in Jupyter or VS Code and run the cells.

---

## 🧾 Requirements

```
transformers
torch
Pillow
```

These are listed in `requirements.txt`.

---

## 🖼️ Sample Output

```
Q: What is the cat doing?
A: Sitting

Q: What color is the wall?
A: White

Q: Is the cat sitting or standing?
A: Sitting
```

---

## 📚 References

- [Hugging Face Transformers Documentation](https://huggingface.co/docs/transformers)
- [Salesforce BLIP VQA Model](https://huggingface.co/Salesforce/blip-vqa-base)

---

## 📌 Notes

- Ensure that the image path in the notebook is correct: `"images/cat.jpg"`
- If you have a GPU and CUDA installed, the model will automatically use it for faster inference.