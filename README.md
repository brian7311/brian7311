library(git2r)

repo_url 
<- "https://github.com/meowmix09831/Environmental/"

local_path 
<- "/Users/ETaranenko/Library/Mobile Documents/com~apple~CloudDocs/Documents/work/ulv/colabs/VictorCarmona/raven"

# cloning github into local_path

repo 
<- git2r::clone(repo_url,
local_path)

# now for loop over all .jpeg files

for (pic
in 
list.files(local_path,pattern
= 
".jpeg")) {

image 
<- magick::image_read(paste0(local_path,"/",pic))

}

This should allow you to download from my GitHub to a file of your choosing on your computer- 👋 Hi, I’m @brian7311
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
brian7311/brian7311 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
