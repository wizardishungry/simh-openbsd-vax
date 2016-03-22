OPENBSD_MIRROR="http://mirrors.nycbug.org/pub/OpenBSD/5.8/vax"

task :default => [:download_files]

task :download_files => "tmp" do
  %W[floppy58.fs].each do |file|
    url = "#{OPENBSD_MIRROR}/#{file}"
    path = "#{file}"
    if not File.exists? path
      sh "curl -C - -o #{path} #{url}"
    else
      puts "skipping #{url}"
    end
  end
end
