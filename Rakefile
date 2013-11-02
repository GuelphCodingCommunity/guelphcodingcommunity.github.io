LESS_FOLDER = './less'
CSS_FOLDER = './css'

desc "Compile less to css"
task :less do
    Dir.glob("#{LESS_FOLDER}/*.less") do |less_file|
	css_file = "#{CSS_FOLDER}/" + File.basename(less_file, ".*") + ".css"
        puts "Compiling #{less_file} to #{css_file}"
        status = system("lessc #{less_file} > #{css_file}")
        puts status ? "OK" : "FAILED"
    end
end
