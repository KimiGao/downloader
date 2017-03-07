require "restclient"

task :check do
  p "========== Check Begin      =========="
  $url = RestClient.get("https://raw.githubusercontent.com/KimiGao/downloader/master/download_link").strip
  p "========== Check Success    =========="
end

task download: :check do
  p "========== Download Begin   =========="
  system("aria2c -d /Users/kimi/Downloads '#{$url}'")
  p "========== Download Success =========="
end
