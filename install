#!/bin/bash

echo "Installing Server Mods and Configs. This will delete the mods folder"

while true; do
    read -p "Do you wish to install this program?" yn
    case $yn in
        [Yy]* ) make install; break;;
        [Nn]* ) exit;;
        * ) echo "Please answer yes or no.";;
    esac
done

echo "Deleting mods folder..."
rm ../mods/*.jar
echo "Done"

echo "Copying mods..."
cp ./mods/*.* ../mods/
echo "Done"

echo "Copying server configs..."
cp ./server-configs/*.* ../configs
echo "Done"

echo "Copying server world configs..."
cp ./world-server-configs/*.* ../forge_world_v1.18/serverconfig/
echo "Done"
