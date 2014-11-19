#usage: rake post tile='title of post'
desc 'create a new draft post'
task :post do
  title = ENV['title']
  slug = "#{Time.now.strftime('%Y-%m-%d')}-#{title.downcase.gsub(/[^\w]+/, '-')}"

  file = File.join(
    File.dirname(__FILE__),
    '_posts',
    slug + '.markdown'
  )

  File.open(file, "w") do |f|
    f << <<-EOS.gsub(/^    /, '')
    ---
    layout: post
    title: #{title}
    published: false
    category: <choose one: blog thoughts challenge tutorial resource>
    ---

    EOS
  end

  system ("#{ENV['EDITOR']} #{file}")
end
