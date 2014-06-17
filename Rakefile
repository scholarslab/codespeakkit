#! /usr/bin/env ruby

require 'csv'

def slugify(string)
  string.downcase.strip.gsub(/[\W]+/,"-")
end

def decorate(row)
  html = <<-SNIP
    <li id="#{slugify(row['name'])}">
      <img src="#{row['avatar']}">
      <h2>#{row['name']}</h2>
      <p class="byline">#{row['byline']}</p>
      <p class="twitter-handle">#{row['twitter']}</p>
      <p class="bio">#{row['biography']}</p>
    </li>
  SNIP
end

desc "Generate participant markup from CSV file"
task :markup, [:file] do |task, args|

  raise IOError, 'File does not exist' unless File.file?(args[:file])

  @csv = CSV.read(args[:file], headers: true)

  html = ""

  @csv.each do |row|
    html << decorate(row)
  end

  puts html

end


