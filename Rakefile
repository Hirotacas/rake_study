desc "センチをインチに変換"

CC = "gcc"

task :default => "cm_to_inch"

file "cm_to_inch" => "cm_to_inch.o" do |t|
  sh "#{CC} -o #{t.name} #{t.prerequisites[0]}"
end

file "cm_to_inch.o" => "cm_to_inch.c" do |t|
  sh "#{CC} -c #{t.prerequisites[0]}"
end
