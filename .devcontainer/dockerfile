# Usamos la imagen de IRIS Health Community
FROM intersystemsdc/irishealth-community:latest

USER root

# Crear directorio de trabajo y dar permisos
WORKDIR /home/vscode/workspace
RUN chown -R ${ISC_PACKAGE_MGRUSER}:${ISC_PACKAGE_IRISGROUP} /home/vscode/workspace

USER ${ISC_PACKAGE_MGRUSER}

# (Opcional) Aquí podrías añadir comandos para auto-importar tus clases .cls
