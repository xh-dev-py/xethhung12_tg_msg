# Build and deploy
```shell
rm -fr dist/*
python -m build
python twine upload dist/* -u __token__ -p {token}
```

# Usage of simple sending
```shell
python -m xethhung12_tg_msg \
    --receiver-id {receiver-id} \
    --bot-token {bot-token} \
    --msg {message} 
    # --silent [if want the program close normally, eception still print out but return in normal return code]
```

# Usage  of sending through STDIN
```shell
python -m xethhung12_tg_msg \
    --receiver-id {receiver-id} \
    --bot-token {bot-token} \
    --from-stdin {stdin input} 
    # --silent [if want the program close normally, eception still print out but return in normal return code]
```