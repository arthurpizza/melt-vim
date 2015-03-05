# melt-vim
Edit videos with Melt and Vim (or other editor of your choice)

## Basics

melt cops.mov in=100 out=460 \
color:black out=30 copy.png \
in=0 out=90

## Fade

melt clip1.av out=90 \
clip2.av out=90 \
-mix 30 -mixer luma

## Render

-consumer \
avformat:render.mp4 \
vcodec=libx264 b=10M \
acodec=aac ab=256k \
s=1920x1080 r=24
