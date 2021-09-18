// Enviar mensaje tipo lista
const rows = [
 {title: 'Row 1', description: "Descripción 1", rowId:"rowid1"},
 {title: 'Row 2', description: "Descripción 2", rowId:"rowid2"}
]

const sections = [{title: "Section 1", rows: rows}]

const button = {
 buttonText: 'Click Aca!',
 description: "Lista de opciones",

sections: sections,
 listType: 1
}

const sendMsg = await conn.sendMessage(id, button, MessageType.listMessage)




// Enviar botone
const buttons = [
  {buttonId: 'id1', buttonText: {displayText: 'Boton 1'}, type: 1},
  {buttonId: 'id2', buttonText: {displayText: 'Boton 2'}, type: 1}
]

const buttonMessage = {
    contentText: "Mensaje de botón",
    footerText: 'Hello World',
    buttons: buttons,
    headerType: 1
}

const sendMsg = await conn.sendMessage(id, buttonMessage, MessageType.buttonsMessage)
