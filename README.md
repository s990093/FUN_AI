```bash
brew install sdl2 sdl2_gfx sdl2_image sdl2_mixer sdl2_net sdl2_ttf
brew install Caskroom/cask/xquartz
pip3 install .
```

# orther

```bash
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
export PYENV_VIRTUALENV_DISABLE_PROMPT=1
pyenv activate .venv
pyenv shell .venv
pip install git+https://github.com/Muxelmann/pygame.git@patch-1
```

# 練習

```bash
python -m mlgame -f 120 --nd -i ./ml/play.py . --difficulty NORMAL --level 5
python ml/model_train.py
python -m mlgame -f 120 -i ./ml/model_play_classification.py . --difficulty NORMAL --level 5
python -m mlgame -f 120 -i ./ml/model_play_regression.py . --difficulty NORMAL --level 5
```

### racing_car

```bash
python -m mlgame -f 120 -i ml/rl_training_PPO.py ./ --game_type NORMAL --car_num 40 --racetrack_length 10000  --round 20 --sound off
```
