# SyntheticPassportsGenerateSRNET

This program allows to generate dataset of RF passports for machine learning  by [SRNet](https://github.com/youdao-ai/SRNet).

## Installation

    1) Create virtual environment:
        conda create -n <your_virtual_environment_name> python=3.6 -y
        conda activate <your_virtual_environment_name>
        
    2) Build virtual environment:
        pip install -r requirements-cpu.txt

    3) To support GPU calculations build virtual environment in this way: 
        pip install -r requirements-gpu.txt
       Also you need to install cuda 10.1
        
## Prerequisites

* Installed [Python](https://www.python.org/downloads/) >= 3.6 or [Anaconda](https://www.anaconda.com/products/individual) >= 4.10.1
* Web Browser: [Google Chrome](https://www.google.com/chrome) or [Mozilla Firefox](https://www.mozilla.org/en/firefox/new/)
* Dowload web driver to work path (see [ChromeDriver](https://chromedriver.chromium.org/downloads) or [mozilla/geckodriver](https://github.com/mozilla/geckodriver/releases) for more information)

## Generation

Download and extract the model from [disk.](https://drive.google.com/file/d/1HkK4xaj3KGK12FdHImn7gCZsjHIMEDZn/view?usp=sharing)

    1) Run script: 
        python srnet_transform_passports.py  --input_path <input path with images + json markup> --output_path <output path> --model  <path with model> --gpu <number gpu>

For more information launch `python srnet_transform_passports.py -h`. 

## References

* [SRNet - Editing Text in the Wild](https://github.com/youdao-ai/SRNet)
* [SRNet-Datagen](https://github.com/youdao-ai/SRNet-Datagen)
