# Excel-Csv-files
#Getting files from excel sheet using Ruby
require 'csv'/map /write_script = File.new("updatescript.out", "w")
CSV.foreach('book3.csv') do |row1|
/puts row1.inspect/
/puts row1[0] +  row1[1]
puts '--' +row1.join(', ')
puts '-- START : ' +row1[0] if !row1[1].nil?
puts ' 'puts 'update LF$APP_PAYMENT set updatedby=\'Run Team\', enabledflag=\'N\'  'puts 'where canonicalid =  \'' +row1[1] + '\'; ' if !row1[1].nil?
puts 'update lf$app_seec_payoutdetails set  enabledflag=\'N\'  'puts 'where canonicalid =  \'' +row1[2] + '\'; ' if !row1[2].nil?
puts 'update lf$app_seec_payment set  enabledflag=\'N\'  'puts 'where canonicalid =  \'' +row1[3] + '\'; ' if !row1[3].nil?
