# setup
## install yabai
brew install koekeishiya/formulae/yabai
brew install koekeishiya/formulae/skhd

## setup config paths
mkdir -p ~/.config/skhd
mkdir -p ~/.config/yabai

## configure yabai-settings
cp skhdrc ~/.config/skhd/skhdrc
cp yabairc ~/.config/yabai/yabairc

## give executable permissions to the yabai script
chmod +x ~/.config/yabai/yabairc

## start skhd and yabai
yabai --start-service
skhd --start-service
