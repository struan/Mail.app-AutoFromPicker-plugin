Every now and again Apple changes the UUIDs for Mail and Messages and
the new ones need to be added to the list in setup.py. To get the UUIDs
run the following commands:

cat /Applications/Mail.app/Contents/Info.plist |grep UUID -A 1 | grep UUID -A 1

cat /System/Library/Frameworks/Message.framework/Resources/Info.plist | grep UUID -A 1
