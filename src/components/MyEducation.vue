<template>
    <dialog id="my_modal_1" class="modal">
        <div class="modal-box md:max-w-1/2">
            <h3 class="text-lg font-bold">FORMACIÓN</h3>

            <div class="collapse collapse-plus bg-base-100 border border-base-300">
                <input type="radio" name="my-accordion-3" />
                <div class="collapse-title font-semibold">
                    Ingeniería de Sistemas
                </div>
                <div class="collapse-content text-sm"> Universidad Nacional Abierta y a Distancia (UNAD) (2022 -
                    Actualidad) <br>
                    Estudios en progreso enfocados en el diseño, desarrollo y gestión de sistemas
                    tecnológicos.
                </div>
            </div>
            <div class="collapse collapse-plus bg-base-100 border border-base-300">
                <input type="radio" name="my-accordion-3" />
                <div class="collapse-title font-semibold">Desarrollo de Aplicaciones Web</div>
                <div class="collapse-content text-sm"> Universidad Tecnológica de Pereira (UTP) (04/2022 - 12/2022)
                    <br>
                    Formación especializada en la creación de aplicaciones web funcionales y
                    escalables.
                </div>
            </div>
            <div class="collapse collapse-plus bg-base-100 border border-base-300">
                <input type="radio" name="my-accordion-3" />
                <div class="collapse-title font-semibold">Desarrollo Frontend con React</div>
                <div class="collapse-content text-sm"> Alura (01/2023 - 06/2023)<br>
                    Capacitación intensiva en el desarrollo de interfaces de usuario interactivas y
                    modernas utilizando React.
                </div>
            </div>
            <div class="collapse collapse-plus bg-base-100 border border-base-300">
                <input type="radio" name="my-accordion-3" />
                <div class="collapse-title font-semibold">Desarrollo Fullstack</div>
                <div class="collapse-content text-sm"> Launch X (02/2022 - 05/2022)<br>
                    Aprendizaje práctico en tecnologías como, JavaScript, Vue.js…
                </div>
            </div>
            <form method="dialog" class="flex justify-end mt-1">
                <button class="btn btn-error btn-soft">Cerrar</button>
            </form>
        </div>
    </dialog>
</template>
