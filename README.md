#Task 1
Generate the voice cloining model using the following command using following modules
```
git clone https://github.com/neonbjb/tortoise-tts.git
cd tortoise-tts
python setup.py install
#creating the sample voice for andrew tate by addingthe wav filr in the voice folder
!python tortoise/do_tts.py --text "Hello how are you" --voice tate --preset
fast
```
#Task 2
Working with wav2lip library for lipsyncing
```

git clone https://github.com/justinjohn0306/Wav2Lip

wget 'https://iiitaphyd-my.sharepoint.com/personal/radrabha_m_research_iiit_ac_in/_layouts/15/download.aspx?share=EdjI7bZlgApMqsVoEUUXpLsBxqXbn5z8VTmoxp55YNDcIA' -O '/content/Wav2Lip/checkpoints/wav2lip_gan.pth'
a = !pip install https://raw.githubusercontent.com/AwaleSajil/ghc/master/ghc-1.0-py3-none-any.whl

cd Wav2Lip && pip install -r requirements.txt

wget "https://www.adrianbulat.com/downloads/python-fan/s3fd-619a316812.pth" -O "/content/Wav2Lip/face_detection/detection/sfd/s3fd.pth"

pip install ffmpeg-python


pad_top =  2
pad_bottom =  10
pad_left =  2
pad_right =  2
rescaleFactor =  1
nosmooth = False

cd Wav2Lip && python inference.py --checkpoint_path checkpoints/wav2lip_gan.pth --face "/content/video2.mp4" --audio "/content/output10 (1).wav" --pads $pad_top $pad_bottom $pad_left $pad_right --resize_factor $rescaleFactor --nosmooth $nosmooth
```
