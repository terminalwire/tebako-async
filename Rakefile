task :brew do
  sh "brew bundle"
end

task :bundle do
  sh "bundle"
end

task :press do
  sh "tebako press -r async -e binance.rb -o tebako-binance-package"
end

task default: %i[brew bundle press]
