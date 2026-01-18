# HeartMuLa_ComfyUI
ComfyUI Custom Node for HeartMuLa AI Music Generation and Transcript Text

------------------------------------------------------------

# Installation

------------------------------------------------------------

**Step 1**

Go to ComfyUI\custom_nodes
Command prompt:

git clone https://github.com/benjiyaya/HeartMuLa_ComfyUI

**Step 2**

cd /HeartMuLa_ComfyUI

**Step 3**

pip install -r requirements.txt

------------------------------------------------------------

# For File structure

------------------------------------------------------------

ComfyUI/custom_nodes/HeartMuLa_ComfyUI/
├── __init__.py                <-- The code provided below
├── util/                      <-- Create this folder
│   └── heartlib/              <-- Paste the heartlib SOURCE CODE here
│       ├── __init__.py
│       ├── pipelines.py
│       ├── models.py
│       └── ... (other python files)
└── requirements.txt           (Optional: torch, transformers, torchaudio, etc.)


------------------------------------------------------------

# Download model files

------------------------------------------------------------
Go to ComfyUI/models 

Use HuggingFace Cli donwload model weigths.

type :

hf download --local-dir './HeartMuLa' 'HeartMuLa/HeartMuLaGen'

hf download --local-dir './HeartMuLa/HeartMuLa-oss-3B' 'HeartMuLa/HeartMuLa-oss-3B'

hf download --local-dir './HeartMuLa/HeartCodec-oss' 'HeartMuLa/HeartCodec-oss'

hf download --local-dir './HeartMuLa/HeartTranscriptor-oss' 'HeartMuLa/HeartTranscriptor-oss' 


------------------------------------------------------------

# For Model File structure

------------------------------------------------------------
ComfyUI/
└── models/
    └── HeartMuLa/
        ├── gen_config.json
        ├── tokenizer.json
        ├── HeartCodec-oss/
        ├── HeartMuLa-oss-3B/
        └── HeartMuLa-oss-7B/ (Jan 2026 not release yet, will update this node once 7B publish.)


------------------------------------------------------------



