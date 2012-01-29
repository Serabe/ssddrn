# A sample Guardfile
# More info at https://github.com/guard/guard#readme

guard 'shell' do
  watch(%r{(.+)\.tex}) do |m|
    #`growlnotify -m #{m[0]} Recompiling`
    `pdflatex -interaction=batchmode -output-directory=out #{m[0]} >/dev/null`
  end
end
