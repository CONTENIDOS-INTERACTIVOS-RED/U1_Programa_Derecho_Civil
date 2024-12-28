<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from '@/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema: 'Fuentes y Personas del Derecho Civil',
      titulo: 'Cuestionario',
      introduccion:
        '<b>Objetivo:</b> Identificar y comprender las fuentes del Derecho Civil colombiano y los conceptos fundamentales sobre personas naturales y jurídicas.',
      barajarPreguntas: true,
      preguntas: [
        {
          id: 1,
          texto:
            'María está asesorando a un cliente sobre la validez de un contrato de compra de una propiedad. Durante la consulta, el cliente le cuenta que en la inmobiliaria es normal adelantar trámites sin la firma del contrato, y que todos han validado esta conducta. María le explica a su cliente que esa conducta no hace que exista validez, incluso si es costumbre. En esta situación, ¿Cuál es la fuente esencial del Derecho Civil que regula los contratos en Colombia?',
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'La ley', esCorrecta: true },
            { id: 'b', texto: 'La costumbre', esCorrecta: false },
            { id: 'c', texto: 'La jurisprudencia', esCorrecta: false },
            { id: 'd', texto: 'La doctrina', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 2,
          texto:
            'Jorge es juez civil y en el marco de un proceso legal es cuestionado por la prensa al no basar su decisión en la jurisprudencia de casos previos. En entrevista con los medios de comunicación el juez explica que no puede hacerlo, ya que existen otras fuentes que son primarias y vinculantes. De acuerdo con lo señalado por Jorge, ¿Cuál es el papel de la jurisprudencia en el Derecho Civil colombiano?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Es la principal fuente obligatoria',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Es fuente auxiliar, no obligatoria',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Es una fuente de derecho en todos los casos',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Prevalece sobre la ley escrita',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto:
            'Alejandro, dueño de una empresa familiar, está creando una nueva sociedad. Durante este proceso, se enfrenta a la duda de si su empresa debe considerarse una persona natural o una persona jurídica según el Derecho Civil colombiano. Alejandro se pregunta cuál es la diferencia clave entre los dos tipos de personas. ¿Cuál es la diferencia fundamental entre una persona natural y una persona jurídica según el Derecho Civil colombiano?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'La persona natural tiene derechos individuales, mientras que la persona jurídica no tiene derechos',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'La persona jurídica puede ser creada por una persona natural sin necesidad de un documento legal',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La persona natural es un ser humano, mientras que la persona jurídica es una entidad creada por la ley para representar intereses colectivos',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'La persona natural está obligada a registrar su existencia, mientras que la persona jurídica no',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto:
            'Clara, gerente de una empresa, está revisando los estatutos de la compañía y se da cuenta que no se menciona si la empresa puede adquirir propiedades. Se pregunta si, como persona jurídica, la empresa tiene la capacidad de poseer bienes y realizar actos jurídicos. ¿Qué derecho tiene una persona jurídica en cuanto a la adquisición de bienes según el Derecho Civil colombiano?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Puede adquirir bienes y realizar actos jurídicos en función de su objeto social y estatutos',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Solo puede poseer bienes si es una entidad pública',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La adquisición de bienes debe ser aprobada por una persona natural',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Las personas jurídicas no pueden adquirir bienes inmuebles',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto:
            'Julián, abogado de una multinacional, está revisando los contratos internacionales de su empresa y se da cuenta de que una de las partes es una empresa pública extranjera. Se pregunta si, en Colombia, las entidades públicas también son consideradas personas jurídicas. ¿Las entidades públicas se consideran personas jurídicas según el Derecho Civil colombiano?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Sí, son personas jurídicas de derecho público',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'No, solo las entidades privadas tienen personalidad jurídica',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Las entidades públicas son consideradas personas naturales',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Solo las entidades privadas y sin ánimo de lucro tienen personalidad jurídica',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
