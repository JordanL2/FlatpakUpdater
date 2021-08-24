 # Flatpak Updater
 
 Given a flatpak manifest as the first and only option, it will:
 
 * Go through every source in every module (top level modules only, currently)
 * For every source that is an archive, and has a URL pointing to Github, check if there is a new release available for that repo
 * If there is, replace the URL of the github archive with a URL for the newer release
 * Also update the sha256 sum with the sum for the newer release
 