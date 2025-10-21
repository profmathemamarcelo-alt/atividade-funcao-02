<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Atividade - GeoGebra: Função Modular</title>

  <!-- Tailwind sem preflight (preserva CSS base) -->
  <script>
    window.tailwind = window.tailwind || {};
    tailwind.config = { corePlugins: { preflight: false } };
  </script>
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- QRCode + jsPDF -->
  <script src="https://cdn.jsdelivr.net/npm/qrcode@1.5.3/build/qrcode.min.js" defer></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js" defer></script>

  <style>
    .error { border-color: #ef4444 !important; }
    button:disabled { opacity:.6; cursor:not-allowed; }
    /* micro-detalhes visuais */
    .card { border:1px solid rgb(226 232 240); box-shadow: 0 6px 20px rgba(2,6,23,.06); }
    .badge { font-size:.75rem; padding:.125rem .5rem; border-radius:9999px; border:1px solid rgba(2,6,23,.1);}
  </style>
</head>
<body class="bg-slate-50 text-slate-800">
  <div class="max-w-3xl mx-auto p-6">
    <header class="mb-6 border-b border-slate-200 pb-4 flex items-center justify-between">
      <div>
        <h1 class="text-2xl font-bold text-indigo-700">Atividade de Matemática – Funções Modulares</h1>
        <p class="text-sm text-slate-600">Prof.: Marcelo P. Antônio</p>
      </div>
      <span class="badge bg-indigo-50 text-indigo-700">GeoGebra</span>
    </header>

    <form id="atividade-form" class="space-y-6 bg-white p-6 rounded-xl card" novalidate>
      <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
        <div>
          <label class="block text-sm font-medium">Nome:</label>
          <input type="text" name="nome" class="w-full border border-slate-300 px-3 py-2 rounded-md" required />
        </div>
        <div>
          <label class="block text-sm font-medium">Turma:</label>
          <input type="text" name="turma" class="w-full border border-slate-300 px-3 py-2 rounded-md" required />
        </div>
      </div>

      <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
        <div>
          <label class="block text-sm font-medium">1) Equação modular — 01 (a):</label>
          <input type="text" name="funcao" class="w-full border border-slate-300 px-3 py-2 rounded-md" required />
        </div>
        <div>
          <label class="block text-sm font-medium">2) Equação modular — 01 (b):</label>
          <input type="text" name="q1" class="w-full border border-slate-300 px-3 py-2 rounded-md" />
        </div>
        <div>
          <label class="block text-sm font-medium">3) Equação modular — 01 (c):</label>
          <input type="text" name="q2" class="w-full border border-slate-300 px-3 py-2 rounded-md" />
        </div>
        <div>
          <label class="block text-sm font-medium">4) Solução do item (a):</label>
          <input type="text" name="q3" class="w-full border border-slate-300 px-3 py-2 rounded-md" />
        </div>
        <div>
          <label class="block text-sm font-medium">5) Solução do item (b):</label>
          <input type="text" name="q4" class="w-full border border-slate-300 px-3 py-2 rounded-md" />
        </div>
        <div>
          <label class="block text-sm font-medium">6) Solução do item (c):</label>
          <input type="text" name="q5" class="w-full border border-slate-300 px-3 py-2 rounded-md" />
        </div>
      </div>

      <div>
        <label class="block text-sm font-medium">7) Link da atividade no GeoGebra:</label>
        <input id="q10-link" type="url" name="q10-link" placeholder="https://..." required class="w-full border border-slate-300 px-3 py-2 rounded-md mb-1" />
        <p id="url-help" class="text-xs text-rose-600 hidden">Insira uma URL válida (http:// ou https://)</p>

        <!-- Prévia do link (bonita e útil) -->
        <div id="link-preview" class="mt-3 hidden">
          <div class="flex items-start gap-3 p-3 rounded-lg border border-slate-200 bg-slate-50/60">
            <img id="lp-fav" alt="" class="w-6 h-6 rounded-sm border border-slate-200 bg-white">
            <div class="min-w-0">
              <div class="text-sm font-medium text-slate-800 truncate" id="lp-title">Título da página</div>
              <div class="text-xs text-slate-500 truncate" id="lp-host">domínio</div>
              <a id="lp-open" href="#" target="_blank" rel="noopener" class="inline-flex items-center gap-1 mt-1 text-xs text-indigo-700 underline">
                Abrir no navegador
                <svg xmlns="http://www.w3.org/2000/svg" class="w-3 h-3" viewBox="0 0 24 24" fill="currentColor"><path d="M14 3h7v7h-2V6.41l-9.29 9.3-1.42-1.42 9.3-9.29H14V3Z"/><path d="M5 5h5V3H3v7h2V5Zm0 14v-5H3v7h7v-2H5Z"/></svg>
              </a>
            </div>
          </div>
        </div>

        <div class="mt-3 flex items-center gap-4">
          <canvas id="qrcode" width="160" height="160" class="border rounded-md bg-white"></canvas>
          <div class="text-xs text-slate-500">
            <p>QR Code para acesso rápido.</p>
            <p id="qr-msg" class="text-rose-600 mt-1 hidden"></p>
          </div>
        </div>
      </div>

      <div class="pt-2 flex flex-wrap gap-3 justify-end">
        <button id="btn-enviar" type="submit" class="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700">Gerar PDF</button>
        <button type="reset" class="px-4 py-2 bg-gray-100 text-slate-700 rounded-lg hover:bg-gray-200">Limpar</button>
      </div>
    </form>

    <div id="download-area" class="mt-6 hidden">
      <div class="flex flex-wrap items-center gap-3 bg-emerald-50 border border-emerald-200 text-emerald-800 px-4 py-3 rounded-lg">
        <p class="text-sm font-semibold">PDF gerado com sucesso:</p>
        <a id="download-link" href="#" download class="underline font-medium">Baixar novamente</a>
        <button id="download-open" type="button" class="px-3 py-1.5 text-sm bg-emerald-600 text-white rounded-md">Abrir</button>
        <button id="share-btn" type="button" class="px-3 py-1.5 text-sm bg-indigo-600 text-white rounded-md">Compartilhar</button>
        <button id="copy-page-link" type="button" class="px-3 py-1.5 text-sm bg-slate-800 text-white rounded-md">Copiar link da página</button>
      </div>
    </div>

    <p class="text-[11px] text-slate-400 mt-4">Dica: teste o PDF no Adobe Reader ou no viewer nativo do navegador para garantir que o link esteja clicável.</p>
  </div>

  <script defer>
  (function(){
    try{
      const $ = (s)=>document.querySelector(s);
      function isValidURL(str){ try{ const u=new URL(str); return ['http:','https:'].includes(u.protocol);}catch{return false;} }
      function clearCanvas(c){ const ctx=c.getContext('2d'); if(ctx) ctx.clearRect(0,0,c.width,c.height); }
      function loadScript(src, timeoutMs=6000){ 
        return new Promise((res)=>{ 
          const s=document.createElement('script'); let done=false; 
          const t=setTimeout(()=>{ if(done) return; done=true; console.warn('Timeout carregando', src); res(false); }, timeoutMs); 
          s.src=src; s.crossOrigin='anonymous'; s.referrerPolicy='no-referrer'; 
          s.onload=()=>{ if(done) return; done=true; clearTimeout(t); res(true); }; 
          s.onerror=()=>{ if(done) return; done=true; clearTimeout(t); res(false); }; 
          document.head.appendChild(s); 
        }); 
      }
      function pdfSafe(str){ return (str||'').replace(/Δ/g,'Delta'); }
      function sanitizeFilename(str){ return (str||'').normalize('NFD').replace(/[^\w\s-]/g,'').trim().replace(/\s+/g,'-').toLowerCase(); }

      // ---------- QR infra ----------
      let _qrReadyPromise=null;
      async function ensureQRCode(){
        if (_qrReadyPromise) return _qrReadyPromise;
        _qrReadyPromise = (async()=>{
          if (window.QRCode && typeof window.QRCode.toCanvas==='function') return 'modern';
          if (window.QRCode && typeof window.QRCode==='function' && !window.QRCode.toCanvas) return 'classic';
          const sources = [
            'https://cdn.jsdelivr.net/npm/qrcode@1.5.3/build/qrcode.min.js',
            'https://unpkg.com/qrcode@1.5.3/build/qrcode.min.js'
          ];
          for (const url of sources){
            const ok = await loadScript(url);
            if (ok && window.QRCode && typeof window.QRCode.toCanvas==='function') return 'modern';
          }
          const okClassic = await loadScript('https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js');
          if (okClassic && window.QRCode) return 'classic';
          return null;
        })();
        return _qrReadyPromise;
      }

      function toCanvasCompat(canvas, text, opts){
        try{
          const fn = window.QRCode && window.QRCode.toCanvas; 
          if(!fn) return Promise.reject(new Error('toCanvas indisponível'));
          const maybe = fn(canvas, text, opts);
          if (maybe && typeof maybe.then==='function') return maybe;
          return new Promise((resolve, reject)=> fn(canvas, text, opts, (err)=> err?reject(err):resolve()));
        }catch(e){ return Promise.reject(e); }
      }

      async function drawQRToCanvas(canvas, text){
        const mode = await ensureQRCode(); 
        if(!mode) throw new Error('Biblioteca de QR indisponível');
        const ctx = canvas.getContext('2d'); if(!ctx) throw new Error('Canvas 2D não disponível');
        clearCanvas(canvas);

        if (mode === 'modern' && typeof window.QRCode.toCanvas==='function'){
          await toCanvasCompat(canvas, text, { width:160, margin:1 });
          return canvas.toDataURL('image/png');
        }
        const tmp = document.createElement('div');
        new window.QRCode(tmp, { text, width:160, height:160, correctLevel: window.QRCode.CorrectLevel ? window.QRCode.CorrectLevel.M : undefined });
        await new Promise(r=>setTimeout(r,140));
        let srcCanvas = tmp.querySelector('canvas');
        if (!srcCanvas){
          const img = tmp.querySelector('img'); if(!img) throw new Error('QR não gerado (fallback)');
          canvas.width = img.naturalWidth || 160; canvas.height = img.naturalHeight || 160; ctx.drawImage(img,0,0,canvas.width,canvas.height);
          return canvas.toDataURL('image/png');
        }
        canvas.width = srcCanvas.width; canvas.height = srcCanvas.height; ctx.drawImage(srcCanvas,0,0);
        return canvas.toDataURL('image/png');
      }

      // ---------- DOM elems ----------
      const form=$('#atividade-form');
      const linkInput=$('#q10-link');
      const qrCanvas=$('#qrcode');
      const urlHelp=$('#url-help');
      const qrMsg=$('#qr-msg');
      const previewWrap=$('#link-preview');
      const lpFav=$('#lp-fav');
      const lpTitle=$('#lp-title');
      const lpHost=$('#lp-host');
      const lpOpen=$('#lp-open');

      const downloadArea=$('#download-area');
      const downloadLink=$('#download-link');
      const downloadOpen=$('#download-open');
      const submitBtn=$('#btn-enviar');
      const shareBtn=$('#share-btn');
      const copyPageBtn=$('#copy-page-link');

      let qrImageDataURL='';
      let currentPdfUrl=null;
      const isiOS = /iPad|iPhone|iPod/.test(navigator.userAgent) || (navigator.platform==='MacIntel' && navigator.maxTouchPoints>1);

      // ---------- Link Preview bonito ----------
      async function updateLinkPreview(){
        const val = linkInput.value.trim();
        if(!val || !isValidURL(val)){
          previewWrap.classList.add('hidden');
          return;
        }
        const u = new URL(val);
        const host = u.hostname;
        const favicon = `https://www.google.com/s2/favicons?sz=64&domain=${encodeURIComponent(host)}`;
        lpFav.src = favicon;
        lpHost.textContent = host;
        lpOpen.href = val;

        // Tentar obter um título curto (pode falhar por CORS)
        let title = '';
        try{
          const res = await fetch(val, { method:'GET', mode:'cors' });
          if (res.ok){
            const html = await res.text();
            const doc = new DOMParser().parseFromString(html, 'text/html');
            title = (doc.querySelector('meta[property="og:title"]')?.content
                  || doc.querySelector('title')?.textContent || '').trim();
          }
        }catch(_){ /* CORS pode bloquear. Tudo bem. */ }
        if(!title){
          // fallback: última parte do path ou domínio
          const path = u.pathname.split('/').filter(Boolean);
          title = (path[path.length-1] || host).replace(/[-_]/g,' ').slice(0,80);
        }
        lpTitle.textContent = title;
        previewWrap.classList.remove('hidden');
      }

      // ---------- QR regen + validação ----------
      async function regenerateQR(){
        try{
          qrImageDataURL='';
          qrMsg.classList.add('hidden'); qrMsg.textContent='';
          const val=linkInput.value.trim();

          await updateLinkPreview();

          if(!val){
            urlHelp.classList.add('hidden'); linkInput.classList.remove('error');
            clearCanvas(qrCanvas); submitBtn.disabled=false; return;
          }
          if(!isValidURL(val)){
            urlHelp.classList.remove('hidden'); linkInput.classList.add('error');
            clearCanvas(qrCanvas); submitBtn.disabled=true; return;
          }
          urlHelp.classList.add('hidden'); linkInput.classList.remove('error'); submitBtn.disabled=true;

          const attempts = 3; let lastErr=null;
          for (let i=0;i<attempts;i++){
            try {
              await ensureQRCode();
              qrImageDataURL = await drawQRToCanvas(qrCanvas, val);
              if (qrImageDataURL){ submitBtn.disabled=false; return; }
            } catch(e){ lastErr=e; await new Promise(r=>setTimeout(r, 200*(i+1))); }
          }
          console.error('Falha QR após tentativas:', lastErr);
          qrMsg.textContent='Falha ao gerar QR. Verifique o link e a conexão, depois tente novamente.';
          qrMsg.classList.remove('hidden');
          clearCanvas(qrCanvas);
          submitBtn.disabled=false;
        }catch(err){ console.error('Erro regenerateQR:', err); }
      }

      linkInput.addEventListener('input', regenerateQR);
      linkInput.addEventListener('change', regenerateQR);
      linkInput.addEventListener('blur', regenerateQR);
      linkInput.addEventListener('paste', ()=> setTimeout(regenerateQR,0));
      document.addEventListener('DOMContentLoaded', async ()=>{ if(linkInput.value && linkInput.value.trim()) regenerateQR(); });

      // ---------- Helpers PDF ----------
      function addPageIfNeeded(doc, y, extra, pageHeight, margin){
        if (y.current + extra > pageHeight - margin){
          doc.addPage();
          y.current = margin;
        }
      }

      function writeField(doc, label, value, opts, layout){
        const { margin, usable, pageHeight } = layout;
        const y = layout.y;
        const isLink = !!opts.link;
        const linkLabel = opts.linkLabel || 'Abrir atividade no GeoGebra';
        const showUrlBelow = opts.showUrlBelow ?? true;

        // Label
        doc.setFont('helvetica','bold'); doc.setFontSize(12); doc.setTextColor(0);
        const labelLines = doc.splitTextToSize(pdfSafe(label), usable);
        for (const ln of labelLines){ addPageIfNeeded(doc, y, 14, pageHeight, margin); doc.text(ln, margin, y.current); y.current += 14; }

        const raw = (value ?? '—').toString().trim();

        if (!isLink) {
          doc.setFont('helvetica','normal'); doc.setFontSize(11); doc.setTextColor(0);
          const valueLines = doc.splitTextToSize(pdfSafe(raw), usable);
          for (const ln of valueLines){ addPageIfNeeded(doc, y, 18, pageHeight, margin); doc.text(ln, margin, y.current); y.current += 18; }
          y.current += 6; addPageIfNeeded(doc, y, 0, pageHeight, margin);
          return;
        }

        // Link curto (clicável) + URL em cinza abaixo (opcional)
        const url = raw;

        // Linha do link (azul + sublinhado)
        doc.setFont('helvetica','normal'); doc.setFontSize(11); doc.setTextColor(0,102,204);
        const shortText = linkLabel;
        addPageIfNeeded(doc, y, 14, pageHeight, margin);
        if (typeof doc.textWithLink === 'function'){
          doc.textWithLink(shortText, margin, y.current, { url });
        } else {
          doc.text(shortText, margin, y.current);
          const w = doc.getTextWidth(shortText);
          doc.link(margin, y.current-8, w, 12, { url });
        }
        // Sublinha
        const wline = doc.getTextWidth(shortText);
        doc.setDrawColor(0,102,204);
        doc.line(margin, y.current+2, margin + wline, y.current+2);
        y.current += 16;

        // URL cinza pequena (auditoria)
        if (showUrlBelow){
          doc.setFont('helvetica','normal'); doc.setFontSize(9); doc.setTextColor(120);
          const urlLines = doc.splitTextToSize(url, usable);
          for (const ln of urlLines){ addPageIfNeeded(doc, y, 12, pageHeight, margin); doc.text(ln, margin, y.current); y.current += 12; }
        }
        y.current += 6; 
        doc.setTextColor(0);
        addPageIfNeeded(doc, y, 0, pageHeight, margin);
      }

      // ---------- Submit ----------
      form.addEventListener('submit', async (e)=>{
        e.preventDefault();
        try{
          const urlVal=linkInput.value.trim();
          if(!urlVal || !isValidURL(urlVal)){
            urlHelp.classList.remove('hidden'); linkInput.classList.add('error'); linkInput.focus();
            return;
          }
          await regenerateQR();
          if(!qrImageDataURL){
            qrMsg.textContent = 'Não foi possível gerar o QR Code. Verifique o link e sua conexão e tente novamente.';
            qrMsg.classList.remove('hidden');
            linkInput.focus();
            return;
          }

          const fd=new FormData(form); const data={}; fd.forEach((v,k)=>data[k]=v);

          const { jsPDF } = window.jspdf || {}; 
          if(!jsPDF){ alert('Biblioteca de PDF (jsPDF) não carregou.'); return; }

          const doc=new jsPDF({unit:'pt',format:'a4'});
          const pageWidth = doc.internal.pageSize.getWidth();
          const pageHeight = doc.internal.pageSize.getHeight();
          const margin=48; 
          const usable = pageWidth - 2*margin; 
          const y = { current: margin };
          doc.setLineHeightFactor(1.2);

          // Cabeçalho elegante
          doc.setFont('helvetica','bold'); doc.setFontSize(16);
          doc.text('Atividade – Funções Modulares e o GeoGebra', margin, y.current+12, { maxWidth: usable });
          doc.setFont('helvetica','normal'); doc.setFontSize(11);
          doc.text('Data: '+new Date().toLocaleDateString('pt-BR'), pageWidth - margin - 120, y.current+12);
          y.current += 60;

          const layout = { margin, usable, pageHeight, y };

          const fields = [
            {key:'nome', label:'Nome'},
            {key:'turma', label:'Turma'},
            {key:'funcao', label:'1) Escreva a equação modular da questão - 01 (a):'},
            {key:'q1', label:'2) Escreva a equação modular da questão - 01 (b):'},
            {key:'q2', label:'3) Escreva a equação modular da questão - 01 (c):'},
            {key:'q3', label:'4) Qual a solução da equação do item a:'},
            {key:'q4', label:'5) Qual a solução da equação do item b:'},
            {key:'q5', label:'6) Qual a solução da equação do item c:'},
            {key:'q10-link', label:'7) Link do GeoGebra', link:true, linkLabel:'Abrir atividade no GeoGebra', showUrlBelow:true }
          ];

          // Conteúdo
          for(const f of fields){
            writeField(doc, f.label, data[f.key] || '', { link: !!f.link, linkLabel: f.linkLabel, showUrlBelow: f.showUrlBelow }, layout);
          }

          // QR no PDF
          if(qrImageDataURL){ 
            try{ 
              const qrW = 120, qrH = 120;
              if (y.current + qrH > pageHeight - margin) { doc.addPage(); y.current = margin; }
              doc.addImage(qrImageDataURL,'PNG',pageWidth - margin - qrW, y.current-16, qrW, qrH); 
              y.current += qrH;
            }catch(e){ console.warn('QR no PDF:', e); } 
          }

          // Rodapé
          doc.setFontSize(9); doc.setTextColor(120);
          if (y.current + 20 > pageHeight - margin){ doc.addPage(); y.current = margin; }
          doc.text('Gerado automaticamente pelo formulário do Prof. Marcelo', margin, pageHeight - margin/2);

          const filename = `atividade-funcao-modular-${sanitizeFilename(data.turma)}-${sanitizeFilename(data.nome)}.pdf`;

          // Download/abertura
          try{
            const blob = doc.output('blob');
            if(currentPdfUrl) { try{ URL.revokeObjectURL(currentPdfUrl); }catch(e){} }
            currentPdfUrl = URL.createObjectURL(blob);
            downloadLink.href = currentPdfUrl; 
            downloadLink.target = "_blank";
            downloadLink.rel = "noopener";
            downloadLink.download = filename; 
            downloadLink.textContent = filename;
            downloadArea.classList.remove('hidden');

            if(isiOS){
              window.open(currentPdfUrl, '_blank');
            } else {
              const a=document.createElement('a'); 
              a.href=currentPdfUrl; 
              a.target="_blank";
              a.rel="noopener";
              a.download=filename; 
              document.body.appendChild(a); 
              a.click(); 
              a.remove();
            }
          }catch(err){ 
            console.error('Falha no download do PDF:', err); 
            try{ doc.save(filename); }catch(e){} 
          }
        }catch(err){
          console.error('Erro no submit:', err);
        }
      });

      // ---------- Ações pós-PDF ----------
      downloadOpen.addEventListener('click', ()=>{ if(currentPdfUrl) window.open(currentPdfUrl, '_blank'); });
      shareBtn.addEventListener('click', async ()=>{
        if(!currentPdfUrl) return;
        try{
          const res = await fetch(currentPdfUrl);
          const blob = await res.blob();
          const file = new File([blob], (downloadLink.download || 'atividade.pdf'), { type: 'application/pdf' });
          if(navigator.canShare && navigator.canShare({ files: [file] })){
            await navigator.share({ files: [file], title: 'Atividade – PDF', text: 'Envio do PDF da atividade' });
          } else if(navigator.share){
            await navigator.share({ title: 'Atividade – PDF', url: currentPdfUrl });
          } else {
            alert('Compartilhamento nativo não suportado neste navegador. Use o botão Abrir e envie manualmente.');
          }
        } catch(e){
          console.error('Compartilhar falhou', e);
          alert('Não foi possível compartilhar o PDF. Tente abrir e enviar manualmente.');
        }
      });

      copyPageBtn.addEventListener('click', async ()=>{
        try{
          await navigator.clipboard.writeText(location.href);
          copyPageBtn.textContent = 'Link copiado!'; 
          setTimeout(()=> copyPageBtn.textContent='Copiar link da página', 2000);
        }catch{ 
          alert('Não foi possível copiar. Copie manualmente o endereço da barra do navegador.'); 
        }
      });

    }catch(err){
      console.error('Erro global:', err);
    }
  })();
  </script>
</body>
</html>
