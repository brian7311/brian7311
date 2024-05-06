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


