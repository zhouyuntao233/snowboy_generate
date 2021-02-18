# snowboy_generate
- Record 3 wav files (16000 sample rate, 16 bits, 1 channel), each with one hotword, e.g.,

```shell
rec -r 16000 -c 1 -b 16 -e signed-integer -t wav record1.wav
```

- Run the following command to train your personal model

```shell
python generate_pmdl.py -r1=record1.wav -r2=record2.wav -r3=record3.wav -lang=en -n=hotword.pmdl
```
