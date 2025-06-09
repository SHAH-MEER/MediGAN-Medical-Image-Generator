# MediGan

MediGan is a Streamlit-based application for generating synthetic medical images using a variety of pre-trained GAN (Generative Adversarial Network) models. The app leverages the [medigan](https://github.com/RichardObi/medigan) library and provides a simple UI for selecting models and generating images.

## Features
- Select from multiple pre-trained GAN models for different medical imaging tasks (e.g., mammography, MRI, chest X-ray)
- Generate a user-defined number of synthetic images
- View generated images directly in the web interface

## Available Models
The following model IDs are available:
- 00001_DCGAN_MMG_CALC_ROI
- 00002_DCGAN_MMG_MASS_ROI
- 00003_CYCLEGAN_MMG_DENSITY_FULL
- 00004_PIX2PIX_MMG_MASSES_W_MASKS
- 00007_INPAINT_BRAIN_MRI
- 00019_PGGAN_CHEST_XRAY
- 00021_CYCLEGAN_BRAIN_MRI_T1_T2
- 00022_WGAN_CARDIAC_AGING

## Getting Started

### Prerequisites
Install the required Python packages (preferably in a virtual environment):

```bash
pip install -r requirements.txt
```

### Running the App

To launch the Streamlit app, run:

```bash
streamlit run app.py
```

This will open the MediGan interface in your web browser.

## Project Structure

- `app.py` — Main Streamlit application
- `models/` — Contains model-related files
- `notebooks/` — Jupyter notebooks for experiments or demos
- `output/` — Output directory for generated images
- `config/` — Configuration files
- `requirements.txt` — Python dependencies

## Notes
- The app will automatically download or install additional model dependencies as needed via the `medigan` library.
- Some models may require additional downloads on first use, so initial generation may take longer.

## License
This project is for research and educational purposes. See the LICENSE file for more details if available.

## Acknowledgements
- [medigan](https://github.com/RichardObi/medigan)
- [Streamlit](https://streamlit.io/)
- [PyTorch](https://pytorch.org/)
