task :brew do
  sh "brew update"
  sh "brew bundle -f"
end

task :bundle do
  sh "bundle"
end

task :install do
  sh "gem install tebako"
end

task :setup do
  sh "PATH=$(brew --prefix bison)/bin:$PATH tebako setup"
end

task :press do
  sh "tebako press -r async -e binance.rb -o tebako-binance-package"
end

task default: %i[brew bundle install setup press]
