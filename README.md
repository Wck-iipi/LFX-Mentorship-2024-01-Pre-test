# LFX-Mentorship-2024-01-Pre-test
## Framework Execution(whisper.cpp):
I took the following steps to get whisper running on my pc:
- Firstly, I cloned the repository.
 ```
git clone https://github.com/ggerganov/whisper.cpp.git
```
![image](https://github.com/Wck-iipi/LFX-Mentorship-2024-01-Pre-test/assets/110763795/82a1da00-6d84-4983-81e1-0de690ad7134)

- Then I downloaded whisper model pre-converted to ggml format
 ```
bash ./models/download-ggml-model.sh base.en
```
![image](https://github.com/Wck-iipi/LFX-Mentorship-2024-01-Pre-test/assets/110763795/220bd4f2-6285-4e65-9f37-dc1419e1e982)


- Finally, I built the main:
 ```
 make
 ```
- Using this built main file, I wrote command to transcribe audio
 ```
./main -f samples/jfk.wav
```
![image](https://github.com/Wck-iipi/LFX-Mentorship-2024-01-Pre-test/assets/110763795/93bbae82-27c6-428f-ba03-5c245d220a28)
![image](https://github.com/Wck-iipi/LFX-Mentorship-2024-01-Pre-test/assets/110763795/179a92f2-dd68-442f-8b78-98a6e47e6beb)
![image](https://github.com/Wck-iipi/LFX-Mentorship-2024-01-Pre-test/assets/110763795/8d4f71ca-3ee9-47b5-a466-500f146c8694)
![image](https://github.com/Wck-iipi/LFX-Mentorship-2024-01-Pre-test/assets/110763795/d24c758c-d86a-4c29-9320-e194c9967c17)


and this file too(I recorded it)
 ```
 ./main -f /home/varun/Desktop/whisperCheck.mp3
```
![image](https://github.com/Wck-iipi/LFX-Mentorship-2024-01-Pre-test/assets/110763795/65bfda00-386d-41b0-b601-f633477a964e)
![image](https://github.com/Wck-iipi/LFX-Mentorship-2024-01-Pre-test/assets/110763795/43045058-630f-464d-96c9-3c8fbb12fffb)

## Build the wasmedge WASI-NN llama.cpp

