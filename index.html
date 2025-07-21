<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Calculadora de Retención - Colombia 2025</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet" />
  <style>
    * { box-sizing: border-box; }
    body {
      font-family: 'Inter', sans-serif;
      background: linear-gradient(135deg, #f0f2f5, #dbe2ef);
      padding: 40px;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      min-height: 100vh;
    }
    .flex-container {
      display: flex;
      gap: 30px;
      justify-content: center;
      align-items: flex-start;
      flex-wrap: wrap;
      max-width: 900px;
      width: 100%;
    }
    .container {
      background-color: #ffffff;
      border-radius: 12px;
      padding: 30px;
      max-width: 420px;
      width: 100%;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    }
    h2 {
      text-align: center;
      margin-bottom: 25px;
      color: #333;
    }
    label {
      font-weight: 600;
      margin-top: 15px;
      display: block;
      color: #444;
    }
    select, input[type="number"], input[type="text"] {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 14px;
      background: #f4f7fa;
      transition: border 0.2s;
    }
    select:focus, input:focus {
      border: 1.5px solid #007bff;
      outline: none;
      background: #eaf2fc;
    }
    .checkbox-label {
      display: flex;
      align-items: center;
      margin-top: 10px;
    }
    .checkbox-label input {
      width: auto;
      margin-right: 10px;
    }
    button {
      background-color: #007bff;
      color: white;
      border: none;
      padding: 12px;
      font-size: 16px;
      width: 100%;
      border-radius: 8px;
      margin-top: 25px;
      cursor: pointer;
      transition: background-color 0.3s, box-shadow 0.3s;
      font-weight: 600;
      box-shadow: 0 2px 8px rgba(0,0,0,0.04);
      letter-spacing: 0.02em;
    }
    button:hover {
      background-color: #0056b3;
      box-shadow: 0 4px 14px rgba(0,123,255,0.12);
    }
    #btn-limpiar {
      background-color: #6c757d !important;
      margin-top: 10px !important;
    }
    #btn-limpiar:hover {
      background-color: #495057 !important;
    }
    #resultado {
      background-color: #f8f9fa;
      padding: 20px;
      border-radius: 10px;
      border-left: 6px solid #007bff;
      min-width: 320px;
      max-width: 350px;
      margin-top: 0;
      height: fit-content;
      display: none;
      box-shadow: 0 5px 18px rgba(0,123,255,0.06);
    }
    #resultado p {
      margin: 8px 0;
      font-size: 15px;
      word-wrap: break-word;
    }
    .valor-grande {
      font-size: 22px;
      font-weight: bold;
      color: #000;
      margin-top: 20px;
    }
    .valor-suave {
      color: #888;
    }
    .total-destacado {
      font-size: 20px;
      font-weight: bold;
      color: #000;
      margin-top: 18px;
    }
    #ica-container {
      display: none;
    }
  </style>
</head>
<body>
  <div class="flex-container">
    <div class="container">
      <h2>Calculadora de Retención 2025</h2>
      <form id="calc-form">
        <label for="quienCompra">¿Quién compra?</label>
        <select id="quienCompra" required>
          <option value="persona_juridica">Persona Jurídica</option>
          <option value="persona_natural">Persona Natural</option>
        </select>

        <label for="quienVende">¿Quién vende?</label>
        <select id="quienVende" required>
          <option value="persona_juridica">Persona Jurídica</option>
          <option value="persona_natural">Persona Natural</option>
        </select>

        <label for="razonSocial">Razón Social (opcional):</label>
        <input type="text" id="razonSocial" placeholder="Ej: Constructora XYZ S.A.S" />

        <label for="responsabilidades">Responsabilidades fiscales:</label>
        <select id="responsabilidades" multiple size="6" required></select>

        <label for="valor">Valor de la operación (sin IVA):</label>
        <input type="number" id="valor" min="0" step="0.01" required />

        <label>Tarifa de IVA:</label>
        <div id="iva-options" style="margin-top: 5px;">
          <label class="checkbox-label"><input type="checkbox" name="iva" value="0.05" /> IVA 5%</label>
          <label class="checkbox-label"><input type="checkbox" name="iva" value="0.19" /> IVA 19%</label>
          <label class="checkbox-label"><input type="checkbox" name="iva" value="0" data-etiqueta="exento" /> Exento</label>
          <label class="checkbox-label"><input type="checkbox" name="iva" value="0" data-etiqueta="excluido" /> Excluido</label>
        </div>

        <div class="checkbox-label">
          <input type="checkbox" id="esBogota" />
          <label for="esBogota">¿La operación se realiza en Bogotá?</label>
        </div>

        <div id="ica-container">
          <label for="tarifaICA">Tarifa ICA Bogotá (‰):</label>
          <select id="tarifaICA">
            <option value="">Seleccione una tarifa</option>
            <option value="4.14">4.14 ‰</option>
            <option value="6.9">6.9 ‰</option>
            <option value="8">8.0 ‰</option>
            <option value="11.04">11.04 ‰</option>
          </select>
        </div>

        <button type="submit">Calcular</button>
        <button type="button" id="btn-limpiar">Limpiar</button>
      </form>
    </div>
    <div id="resultado"></div>
  </div>

  <script>
    const responsabilidadesSelect = document.getElementById('responsabilidades');
    const quienVendeSelect = document.getElementById('quienVende');
    const quienCompraSelect = document.getElementById('quienCompra');
    const razonSocialInput = document.getElementById('razonSocial');
    const valorInput = document.getElementById('valor');
    const esBogotaInput = document.getElementById('esBogota');
    const icaContainer = document.getElementById('ica-container');
    const tarifaICASelect = document.getElementById('tarifaICA');
    const resultadoDiv = document.getElementById('resultado');

    const responsabilidades = {
      persona_juridica: [
        { value: 'O-13', label: 'O-13 - Gran Contribuyente' },
        { value: 'O-15', label: 'O-15 - Autorretenedor' },
        { value: 'O-23', label: 'O-23 - Agente de Retención IVA' },
        { value: 'O-47', label: 'O-47 - Régimen Simple' },
        { value: 'R-99-PN', label: 'R-99-PN - No responsable' },
        { value: 'NINGUNA', label: 'No aplica / Sin responsabilidad' },
      ],
      persona_natural: [
        { value: 'O-47', label: 'O-47 - Régimen Simple' },
        { value: 'R-99-PN', label: 'R-99-PN - No responsable' },
        { value: 'NINGUNA', label: 'No aplica / Sin responsabilidad' },
      ],
    };

    function cargarResponsabilidades(tipoPersona) {
      responsabilidadesSelect.innerHTML = '';
      (responsabilidades[tipoPersona] || []).forEach((opcion) => {
        const option = document.createElement('option');
        option.value = opcion.value;
        option.textContent = opcion.label;
        responsabilidadesSelect.appendChild(option);
      });

      const savedResp = localStorage.getItem('form-responsabilidades');
      if (savedResp) {
        const values = JSON.parse(savedResp);
        Array.from(responsabilidadesSelect.options).forEach(opt => {
          opt.selected = values.includes(opt.value);
        });
      }
    }

    quienVendeSelect.addEventListener('change', () => {
      cargarResponsabilidades(quienVendeSelect.value);
    });

    document.addEventListener('DOMContentLoaded', () => {
      cargarResponsabilidades(quienVendeSelect.value);
      icaContainer.style.display = esBogotaInput.checked ? 'block' : 'none';

      // Restaurar valores del localStorage
      const fields = ['quienCompra', 'quienVende', 'valor', 'razonSocial', 'esBogota', 'tarifaICA'];
      fields.forEach(id => {
        const el = document.getElementById(id);
        const saved = localStorage.getItem(`form-${id}`);
        if (el && saved !== null) {
          el.type === 'checkbox' ? el.checked = saved === 'true' : el.value = saved;
        }
      });

      const savedResp = localStorage.getItem('form-responsabilidades');
      if (savedResp) {
        const values = JSON.parse(savedResp);
        Array.from(responsabilidadesSelect.options).forEach(opt => {
          opt.selected = values.includes(opt.value);
        });
      }
    });

    esBogotaInput.addEventListener('change', () => {
      icaContainer.style.display = esBogotaInput.checked ? 'block' : 'none';
    });

    // Selección única para IVA
    document.querySelectorAll('#iva-options input[type="checkbox"]').forEach(cb => {
      cb.addEventListener('change', function () {
        if (this.checked) {
          document.querySelectorAll('#iva-options input[type="checkbox"]').forEach(other => {
            if (other !== this) other.checked = false;
          });
        }
      });
    });

    document.getElementById('calc-form').addEventListener('submit', function (e) {
      e.preventDefault();

      const valorBase = parseFloat(valorInput.value);
      const tarifaIVASeleccionada = document.querySelector('#iva-options input[type="checkbox"]:checked');
      const tarifaIVA = tarifaIVASeleccionada ? parseFloat(tarifaIVASeleccionada.value) : 0;
      const valorIVA = valorBase * tarifaIVA;
      const valorTotalConIVA = valorBase + valorIVA;

      const esBogota = esBogotaInput.checked;
      const tarifaICASeleccionada = parseFloat(tarifaICASelect.value);
      const responsabilidadesSeleccionadas = Array.from(responsabilidadesSelect.selectedOptions).map(opt => opt.value);
      const quienVende = quienVendeSelect.value;
      const razonSocial = razonSocialInput.value.trim();

      if (responsabilidadesSeleccionadas.length === 0) {
        alert('Debe seleccionar al menos una responsabilidad fiscal.');
        return;
      }

      let reteIVA = 0;
      if (tarifaIVA > 0 && responsabilidadesSeleccionadas.includes('O-23')) {
        reteIVA = valorIVA * 0.15;
      }

      let retefuente = 0;
      let retefuenteLabel = 'No aplica (Autorretenedor)';
      if (!responsabilidadesSeleccionadas.includes('O-15')) {
        const tarifa = quienVende === 'persona_natural' ? 0.035 : 0.025;
        retefuenteLabel = quienVende === 'persona_natural' ? '3.5% (Natural)' : '2.5% (Jurídica)';
        retefuente = valorBase >= 498000 ? valorBase * tarifa : 0;
      }

      let ica = 0;
      let tarifaICA = 0;
      if (esBogota && !isNaN(tarifaICASeleccionada)) {
        tarifaICA = tarifaICASeleccionada;
        ica = valorBase * (tarifaICA / 1000);
      }

      const totalRetenciones = retefuente + reteIVA + ica;
      const valorNeto = valorTotalConIVA - totalRetenciones;

      resultadoDiv.innerHTML = `
        ${razonSocial ? `<p><strong>Razón Social:</strong> ${razonSocial}</p>` : ''}
        <p class="valor-suave"><strong>Valor base:</strong> $${reformat(valorBase)}</p>
        <p class="valor-suave"><strong>IVA (${(tarifaIVA * 100).toFixed(0)}%):</strong> $${reformat(valorIVA)}</p>
        <p class="valor-suave"><strong>Retefuente (${retefuenteLabel}):</strong> $${reformat(retefuente)}</p>
        <p class="valor-suave"><strong>ReteIVA (15% sobre IVA):</strong> $${reformat(reteIVA)}</p>
        <p class="valor-suave"><strong>ICA Bogotá (${tarifaICA.toFixed(2)}‰):</strong> $${reformat(ica)}</p>
        <p class="valor-grande">Total Retenciones: $${Math.round(totalRetenciones).toLocaleString('es-CO')}</p>
        <p class="valor-grande">Valor neto a pagar: $${Math.round(valorNeto).toLocaleString('es-CO')}</p>
      `;
      resultadoDiv.style.display = 'block';
    });

    function reformat(valor) {
      return valor.toLocaleString('es-CO', {
        style: 'decimal',
        minimumFractionDigits: 2,
        maximumFractionDigits: 2,
      });
    }

    document.getElementById('btn-limpiar').addEventListener('click', () => {
      document.getElementById('calc-form').reset();
      resultadoDiv.style.display = 'none';
      cargarResponsabilidades(quienVendeSelect.value);
      icaContainer.style.display = esBogotaInput.checked ? 'block' : 'none';
      localStorage.clear();
    });

    // Guardar datos persistentes
    ['quienCompra', 'quienVende', 'valor', 'razonSocial', 'esBogota', 'tarifaICA'].forEach(id => {
      const el = document.getElementById(id);
      if (el) {
        el.addEventListener('change', () => {
          const value = el.type === 'checkbox' ? el.checked : el.value;
          localStorage.setItem(`form-${id}`, value);
        });
      }
    });

    responsabilidadesSelect.addEventListener('change', () => {
      const selected = Array.from(responsabilidadesSelect.selectedOptions).map(opt => opt.value);
      localStorage.setItem('form-responsabilidades', JSON.stringify(selected));
    });
  </script>
</body>
</html>
