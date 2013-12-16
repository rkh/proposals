file "headshots.md" => FileList['headshots/*'] do |t|
  File.open(t.name, 'w') do |f|
    t.prerequisites.each do |img|
      f.puts "![](#{img})"
    end
  end
end

task default: "headshots.md"
