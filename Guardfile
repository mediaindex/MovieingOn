# A sample Guardfile
# More info at https://github.com/guard/guard#readme

# guard-rackup
# Tha command for rackup
#   :command => "rackup ./config.ru -E development",
#
# start(run :command as above) proc, it must return pid
#   :start => proc{ Process.spawn(command) },
#
# stop proc
#   :stop => proc{|pid| Process.kill("INT", pid); Process.wait pid},
#
# reload proc that fired when watched files changed
#   :reload => proc{ stop; start },
guard "rackup" do
  watch(%r{^(.+)\.rb$})
  watch(%r{^app/.*\.rb$})
  watch(%r{^lib/.*\.rb$})
  watch(%r{^config/.*\.rb$})
  watch("config.ru")
end
