#External Lighting


##com Blender Internal 

###setup 1
Setup 3 Point Lighting (Iluminação de 3 pontos) mas substituir a Key Light por um Sun com Ray (Trace) Shadows.

####3 Point Lighting

Key light é a luz primária, frequentemente colocada a 45 graus em frente e por cima do sujeito. Luz que gera a maior parte da iluminação. Principal função é iluminar os aspectos mais importantes.

Fill light é uma fonte de luz mais suave, ameniza as sombras e contrastes criados pela Luz principal, para iluminar áreas de sombra. Tipicamente colocada do outro lado da câmara e num ângulo de 90º relativamente à key light.

Back light ou rim light (contra-luz) é uma luz forte e brilhante colocada atrás do objeto, utilizada para separar o objeto de interesse do fundo criando uma fina linha de luz ao longo da silhueta do objeto de interesse. Permite destacar os contornos do objecto fazendo com que este se destaque do fundo.

###setup 2
Seguir o setup sugerido acima para a iluminação com 3 pontos mas substituir a Key Light por um Sun com No Shadow e uma Spot com Buffer Shadow e Only Shadow. Esta Spot deverá ter a mesma rotação/direcção do Sun (Sugestão: coloque o Sun, depois duplique-o com Shift+D e altere o duplicado para Spot).

###setup 3
1. Approximate Ambient Occlusion como base.
2. Iluminação direta com Sun.
3. Sombras com Spot, Only Shadow e Buffer Shadow.

##com Cycles 
### setup 1
Sistema mais básico inclui utilizar a cor de Background (sugestão: azul claro tipo #E7EFFF e strength 1-2) + luz Sun. Utilize uma cor amarelada para o Sun, diminua o Shadow Size (sugestão: 0.005) para obter sombras mais nítidas (como num dia de sol) e strength a iniciar no 2.
fonte: https://www.blender3darchitect.com/2012/11/how-to-setup-external-sunlight-for-architecture-with-blender-cycles/

###setup 2
Sun (RGB 1, 0.98, 0.9) + Shadows Size = 0.050 + No World, definir Color para Sky Texture + Ambient Occlusion = 0.25

###setup 3
Utilizar IBL (Image-based lighting) com HDRI.


