# README

Questions faciles
•	Album.all.size
•	Track.find_by(title: "White Room")
              Track.find(505).artist
•	Track.find_by(duration: 188133)
•	a = Album.find_by(title: "Use Your Illusion II")
a.artist

Questions moyennes
•	Album.where("title like ?", "%great%").size
•	Album.where("title like ?", "%music%").destroy_all
•	Album.where(artist: "AC/DC").size
•	Track.where(duration : 158589).size

Questions difficiles
•	Track.where(artist : « AC/DC »).each do |track|
   puts track.title
end
•	Track.where(album : « Let There Be Rock »).each do |track|
  puts track.title
end
•	Track.where(album: "Let There Be Rock").sum(:price)
Track.where(album: "Let There Be Rock").sum(:duration)
•	Track.where(artist: "Deep Purple").sum(:price)
•	Track.where(artist : « Eric Clapton »).each do |track|
  track.update(artist : « Britney Spears »)
end
