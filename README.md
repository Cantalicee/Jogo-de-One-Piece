# Jogo-de-One-Piece
Jogo interativo solo ou em grupo
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  <title>Grand Line: A Era dos Piratas</title>
  <script src="https://unpkg.com/peerjs@1.5.2/dist/peerjs.min.js"></script>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      user-select: none;
      -webkit-user-select: none;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body, html {
      width: 100%;
      height: 100%;
      overflow: hidden;
      background-color: #071928;
      color: #f4ebd9;
    }

    #gameCanvas {
      position: fixed;
      inset: 0;
      width: 100%;
      height: 100%;
      display: block;
      z-index: 1;
      touch-action: none;
    }

    /* Camada Principal de UI */
    #ui-layer {
      position: fixed;
      inset: 0;
      z-index: 10;
      pointer-events: none;
    }

    .interactive {
      pointer-events: auto;
    }

    /* HUD Superior */
    #top-hud {
      position: absolute;
      top: 12px;
      left: 12px;
      right: 12px;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: center;
      gap: 8px;
      pointer-events: none;
    }

    .hud-group {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      align
